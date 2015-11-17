LeMaker Guitar SD Card Image Tool
#################################################################################<br>
Copyright (C) 2015 Saeid Ghazagh <sghazagh@elar-systems.com><br>
<br>
ELAR-Systems<br>
------------<br>
http://www.elar-systems.com<br>
http://www.elar-systems.com.au<br>
<br>
This program is free software; you can redistribute it and/or<br>
modify it under the terms of the GNU General Public License <br>
as published by the Free Software Foundation; either version 2 <br>
of the License, or (at your option) any later version. <br>
 <br>
This program is distributed in the hope that it will be useful, <br>
but WITHOUT ANY WARRANTY; without even the implied warranty of <br>
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the <br>
GNU General Public License for more details. <br>
 <br><br>

Required Packages<br>
-----------------<br>
dd, fdisk, kpartx, bmap-tools
<br>

Usage<br>
------------ <br>
First get a local copy to your machine <br>
$ git clone https://github.com/elar-systems/LeMaker-Guitar<br>

You can make an Image now: <br>
$ cd LeMaker-Guitar <br>
$ ./make-lemaker-guitar-sdcard-img.sh <image_file_name> <br>
<br>
If you are on a Debian based system, you can install bmap-tools <br>
$ sudo apt-get install bmap-tools <br>
 <br>
Extract the archive and use bmaptool to copy it to the SD card <br>
$ sudo bmaptool copy your_sd_image.img /dev/sdX <br>
 <br>
You can also use dd but it will take a lot longer since bmaptool doesn't write the empty bits <br>
Windows users can use "Win32DiskImager" to write the .img file to the SD card <br>
 
