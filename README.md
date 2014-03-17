Install:
apt-get install git g++ python libusb-1.0-0-dev freeglut3-dev openjdk-6-jdk doxygen graphviz

The calc_jobs_number() function in the scripts doesn't seem to work on the Pi, so change python script:

nano ~/stable/OpenNI/Platform/Linux/CreateRedist/Redist_OpenNi.py
from containing this: 

MAKE_ARGS += ' -j' + calc_jobs_number()

to :

MAKE_ARGS += ' -j1'


Must also change the Arm compiler settings for this distribution of the Pi:

nano ~/stable/OpenNI/Platform/Linux/Build/Common/Platform.Arm

from:

CFLAGS += -march=armv7-a -mtune=cortex-a8 -mfpu=neon -mfloat-abi=softfp #-mcpu=cortex-a8

to:

CFLAGS += -mtune=arm1176jzf-s -mfpu=vfp -mfloat-abi=hard


Then run:

cd ~/stable/OpenNI/Platform/Linux/CreateRedist/
./RedistMaker.Arm 

cd ~/stable/OpenNI/Platform/Linux/Redist/OpenNI-Bin-Dev-Linux-Arm-v1.5.2.23

sudo ./install.sh
 

Go to the Redist and run install:

cd ~/stable/OpenNI/Platform/Linux/Redist/OpenNI-Bin-Dev-Linux-Arm-v1.5.4.0

sudo ./install.sh
