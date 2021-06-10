# Install-OpenCV-Jetson-Nano
![output image]( https://qengineering.eu/images/LogoOpenJetsonGitHub.webp )

## OpenCV installation script for a Jetson Nano

[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/>

This is the full setup of OpenCV with CUDA and cuDNN support for the Jetson Nano.<br/>
Without any modification, it can also be used for the Jetson Xavier.<br/>
For more information see [Q-engineering - Install OpenCV Jetson Nano](https://qengineering.eu/install-opencv-4.5-on-jetson-nano.html)

------------

## Installing OpenCV.
```
# check your total memory first you need at least a total of 6.5 GB!
# if not, enlarge your swap space as explained in the guide
$ free -m

$ wget https://github.com/Qengineering/Install-OpenCV-Jetson-Nano/raw/main/OpenCV-4-5-x.sh
$ sudo chmod 755 ./OpenCV-4-5-x.sh
$ ./OpenCV-4-5-x.sh
```
