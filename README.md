# tif2lasTest-exe
Converts Tifs to Las files
usage: tif2las.py [-h] -i INPUT -o OUTPUT [-r] [-c CORES] [--gsupper GSUPPER] [--gslower GSLOWER] [--r1 R1] [--r2 R2]
                  [--b1 B1] [--b2 B2] [--g1 G1] [--g2 G2] [--scale_x SCALE_X] [--scale_y SCALE_Y] [--scale_z SCALE_Z]
                  [--z_step Z_STEP] [--keeptif] [--dcm2tif] [-n CLASSNUMB]

optional arguments:
  -h, --help            show this help message and exit
  -i INPUT, --input INPUT
                        (REQUIRED) input folder
  -o OUTPUT, --output OUTPUT
                        (REQUIRED) output folder
  -r, --rgb             rgb image
  -c CORES, --cores CORES
                        how many cpu cores you want to dedicate
  --gsupper GSUPPER     grayscale cutoff value, upper limit
  --gslower GSLOWER     grayscale cutoff value, lower limit
  --r1 R1               bottom red value for RGB filtering
  --r2 R2               top red value for RGB filtering
  --b1 B1               bottom blue value for RGB filtering
  --b2 B2               top blue value for RGB filtering
  --g1 G1               bottom green for RGB filtering
  --g2 G2               top green for RGB filtering
  --scale_x SCALE_X     scale of x from pdal writers.las options, default .01
  --scale_y SCALE_Y     scale of y from pdal writers.las options, default .01
  --scale_z SCALE_Z     scale of z from pdal writers.las options, default .01
  --z_step Z_STEP       Z step from image to image
  --keeptif             when using dicom2laz keep converted tif
  --dcm2tif             dicom 2 tif
  -n CLASSNUMB, --classnumb CLASSNUMB
                        Total number of classifications to add
