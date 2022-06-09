# Install-OpenCV-Jetson-Nano
![output image]( https://qengineering.eu/images/LogoOpenJetsonGitHub.webp )

## OpenCV installation script for a Jetson Nano

[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/>

This is the full setup of OpenCV with CUDA and cuDNN support for the Jetson Nano.<br/>
For more information see [Q-engineering - Install OpenCV Jetson Nano](https://qengineering.eu/install-opencv-4.5-on-jetson-nano.html)

------------

## Installing OpenCV.
The default memory (4 GB RAM + 2 GB swap) on your Nano is not enough for a quick build.<br/>
In this case the compilation will be done by 1 core, which will take a long time.<br/>
You must have more memory allocated to your Nano for the fast 4 core build.<br/>
```
# check your total memory (RAM + swap) first for a fast build. You need at least a total of:
# OpenCV 4.5.6 -> 8.5 GB!
# OpenCV 4.5.5 -> 8.5 GB!
# OpenCV 4.5.4 -> 8.5 GB!
# OpenCV 4.5.3 -> 8.5 GB!
# OpenCV 4.5.2 -> 8.5 GB!
# OpenCV 4.5.1 -> 6.5 GB
# OpenCV 4.5.0 -> 6.5 GB
# if not, enlarge your swap space as explained in the guide, 
# or only 1 core is used for the compilation.
$ free -m

$ wget https://github.com/Qengineering/Install-OpenCV-Jetson-Nano/raw/main/OpenCV-4-5-x.sh
$ sudo chmod 755 ./OpenCV-4-5-x.sh
$ ./OpenCV-4-5-x.sh
```
:point_right: Don't forget to reset your swap memory afterwards.

------------

If you want to beautify OpenCV with the Qt5 GUI you need to
- $ sudo apt-get install qt5-default
- Set the -D WITH_QT=**ON** \ (± line 62) in the script<br/>
 
before running the script on your Nano

------------

OpenCV will be installed to the `/usr` directory, all files will be copied to following locations:<br/>

- `/usr/bin` - executable files<br/>
- `/usr/lib/aarch64-linux-gnu` - libraries (.so)<br/>
- `/usr/lib/aarch64-linux-gnu/cmake/opencv4` - cmake package<br/>
- `/usr/include/opencv4` - headers<br/>
- `/usr/share/opencv4` - other files (e.g. trained cascades in XML format)<br/>

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 


