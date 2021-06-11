# Install-OpenCV-Jetson-Nano
![output image]( https://qengineering.eu/images/LogoOpenJetsonGitHub.webp )

## OpenCV installation script for a Jetson Nano

[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/>

This is the full setup of OpenCV with CUDA and cuDNN support for the Jetson Nano.<br/>
For more information see [Q-engineering - Install OpenCV Jetson Nano](https://qengineering.eu/install-opencv-4.5-on-jetson-nano.html)

------------

## Installing OpenCV.
You must have allocated more memory than the default on your Nano.<br/>
With the regular 4 GB RAM + 2 GB swap the compilation unfortunately crashes after 2 hours at 100%
```
# check your total memory first you need at least a total of 6.5 GB!
# if not, enlarge your swap space as explained in the guide
$ free -m

$ wget https://github.com/Qengineering/Install-OpenCV-Jetson-Nano/raw/main/OpenCV-4-5-x.sh
$ sudo chmod 755 ./OpenCV-4-5-x.sh
$ ./OpenCV-4-5-x.sh
```
:point_right: Don't forget to reset your swap memory afterwards.
