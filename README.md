Simple Raspberry Pi MMAL project

Build
-----
0. Install pre-required packages
   
    $ sudo apt update
    
    $ sudo apt install cmake libopencv-dev

1. Build pre-required libraries
    
    $ make -C /opt/vc/src/hello_pi/libs/vgfont
    
2. Place  Raspberry Pi userland project in /home/pi/src/raspberrypi/userland
    
    $ mkdir -p /home/pi/src/raspberrypi
    
    $ cd /home/pi/src/raspberrypi
    
    $ git clone --depth 1 https://github.com/raspberrypi/userland.git

3. Build Userland
   
   $ cd /home/pi/src/raspberrypi/userland
   
   $ mkdir build
   
    $ cd build
    
    $ cmake ..
    
    $ make
    
4. Build Project
   
   $ cd /home/pi/src
   
   $ git clone https://github.com/TypeNaN/rpi-mmal-demo.git
   
   $ cd rpi-mmal-demo
   
   $ mkdir build
   
   $ cd build
   
   $ cmake ..
   
   $ make
