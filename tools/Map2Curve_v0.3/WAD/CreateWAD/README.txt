Use this tool by placing it into a folder with BMP files, which were
extracted from a Goldsource WAD directory (e.g. by using Wally) and
whose names contain the necessary informations (width and height) in
the following format:

  ;NAME;WIDTH;HEIGHT;

  For example:
  ;BABTECH_WALL01A;128;128;

IMPORTANT:
This tool can not extract these informations from Bitmap files on its
own. You will still need to add those to the file name via batch
processing software like XnConvert or similar.

XnConvert Filename Convention:
;{Filename};{Width};{Height};

