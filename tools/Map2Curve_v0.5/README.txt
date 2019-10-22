
        ++===========++
        || Map2Curve ||
        ++===========++

        Version: 0.5
        Release: June 30th, 2019
         Author: ToTac
        Contact: totac@web.de
        Website: http://gibshooter.com/
  Documentation: http://gibshooter.com/map2curve/documentation
    v0.5 Manual: http://gibshooter.com/map2curve/version05_overview/
 Special Thanks: voidkeeper (for creating a GUI version of M2C), Admer456 (C++ advice),
		 JoeFortunell (for  his tutorial on the WAD3 format -> http://www.j0e.io),
		 ribcage, Trempler, EnYB0La and others who gave feedback!

   ============= PREAMBLE =============

   This program is a brush generator that currently accepts Goldsource map files as input.
   To create a curved version of a map file it can be dropped onto the executable. For this to work the
   source file has to match certain criteria. Invalid brushes will be ignored.

   WAD information can not be obtained fully automatic. For the program to be able to use your WAD files,
   you have to add the WADs file paths to the WADList.txt in the WAD folder or paste copies of your wad
   files into it. If no texture information could be obtained, the program will use a default texture size.

   ============= BUG REPORTS =============

   Please report any bugs and feature requests to my above mentionend E-Mail, including the specific files
   (map and preset file) and other relevant information (e.g. Operating System).


   ============= Preset Files =============

   Preset files contain various commands that influence the curve generation process. More than one curve
   object can be defined in a preset file. Commands simply stack on top of each other. While no command is
   crucial, the rad (radius) command defines the amount of curves that is being generated.

   For further information about preset files, please take a look into the DEFAULTS.txt or the online documentation:
   -> http://gibshooter.com/map2curve/documentation


   ============= FGD & Entities =============

1. info_curve
   This acts as a source of settings for one curve object. It features the same commands as the so far used
   preset-files. More than one can be created.

2. info_curve_export
   This only contains the export specific commands "target" and "append" and will always overwrite these
   commands from other sources. "source" cant be used here, since map-files will always be their own source-files.
   Only one can be used.

3. info_detailgroup
   This controls individual detail object groups and will overwrite the global settings for those. See below.


   ============= Map Criteria =============

1. Brushwork has to be horizontally aligned along the X-axis and can be anywhere on the map,
   but should be on the top side of the Y-axis. If some vertices of the map-brushes are below 0 on the Y axis,
   the source object will always be moved above 0 on the Y-axis for arc generation.
2. Cut-faces have to be planar.
3. Slopes along the X-axis will lead to an invalid brush.
4. Invalid texture alignments will be aligned to "World" automatically.
5. There can be any entity and type of brush in a Map file.
7. World texture alignment is being transformed to face alignment automatically.


   ============= Detail Objects =============

   Objects (solid and point entities) that are being cloned and aligned along generated curves.
   Add the following commands to any entity (by leaving smart edit in Hammer Editor):
     Key: m2c_d_group
     Value: YourGroupname
   This will create a custom detail group that can have further settings.
   Settings to control the detail groups can be used globally in a usual setting-txt file or info_curve
   entity or by using a personal info_detailgroup entity, that has the same groupname.
   You can also add settings directly to any of the groups member objects
   (IMPORTANT: Add "m2c_" in front of them, e.g. "m2c_d_enable" and use -1 instead of 0, as Hammer will
   not export "0"-values to map-files).

   Lone Wolfs:
   All point entities that don't have any groupname will be treated as lone wolfs and underlie the 
   global settings for detail groups.

   ============= Curve Resolution =============

1. Resolutions for Pi Circles are always divisible by 4. Everything else will be rounded by the program.
   At the moment the minimum resolution is 4.
2. Resolutions for Grid Circles must be 12, 24, 48, 96, 192 or 384 or the appropiate ID: 1(12)...6(384)


   ============= Construction Frames =============

1. Pi Circle
   Uses Pi to generate the construction framework.
   This method will let you turn any brush shape into a curve.

2. Grid Circle
   Uses a special construction method:
   -> http://www.quaketerminus.com/hosted/happymaps/curv_tut.htm
   Low resolutions and simple brushes are recommended!

3. Simple Path Extrusion
   Uses a seperate a path_corner path in a separate map file (can be made in an Editor) to create
   a construction frame from it.
   Filenames must be similar to "mapname_path1.map", where 1 stands for the respective curve object ID.
   Path extrusion can be controlled using further settings.









