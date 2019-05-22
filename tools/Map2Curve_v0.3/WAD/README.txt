
   Map2Curve WAD Rules:

   In case you don't know about WAD-files (Half-Life's texture format),
   they contain a number of texture files (Bitmaps). Map2Curve needs to
   know the dimensions of a texture, to be able to calculate the original
   texture offset and the new shift for export.

   Unfortunately though, Map2Curve can not read real WAD files, so I had to
   go the detour and feed it the needed texture informations through text files.

   Sometimes, when a texture isn't found by searching through the WAD dir,
   it will be given default dimensions (128 pixels wide and high), which
   will probably lead to false texture shifts.

1. Names for Wad Files must begin with "wad_"
   
   Example: wad_halflife.txt

2. Wad Files can be put into a subdirectory for a better view and to avoid filename conflicts.
   Subdirectories must begin with "pack_" to be recognized as such.
   
   Example: pack_valve

3. Correct names for WAD-files are relevant, because they are being compared with the names of the
   WAD files that are actually being used in the map. These are being stored in the map-file itself.
   
   Example: wad_halflife.txt is the Map2Curve counterpart of halflife.wad

4. Textures must be in UPPER CASE and surrounded by ";" and must of course be followed by their
   dimensions width and height, also divided by ";"

   Example:
   Original Texture Name: 	BABTECH_WALL01A, width: 128, height: 128
   WAD-File line:		;BABTECH_WALL01A;128;128;

5. How can you get those texture informations yourself?

   I did it by following these steps:

   a) Open original WAD file in Wally.
   b) Extract all textures as Bitmaps into an empty folder.
   c) Open all these bitmaps with an image batch processing software (I used XnConvert)
   d) Save them again into another folder, while attaching their dimensions to the original
      filename and add the spacers ";" in between.
      In XnConvert: ";{Filename};{Width};{Height};"
   e) Finally you need a way to list all those filenames and copy them into an empty txt-file.
      I did it by using CMD on Windows, change dir (cd) to your 2nd folder, and type "dir",
      to get a list of all the files in this folder, to be able to copy it.
      You still have to get rid of the unnecessary spaces and information. I used Notepad++ to do this.

   I know, this is a real pain in the *** and I will probably write a small program to make it easier soon.













