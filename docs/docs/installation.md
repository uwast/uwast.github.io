#Installing ROS

Installing ROS is rather straight forward, however it must be noted that you have to have Ubuntu 16.04.3 installed on your computer, whether it be a partition or a virtual machine.  We use the ROS Kinetic distribution.  For a detailed guide on install ROS please go [here](http://wiki.ros.org/kinetic/Installation/Ubuntu).

Installing the barebones or desktop version should suffice although you may need to install extra dependancies later.  If you are working on simulators or GUIs at all, get the desktop full installation.

##Installing our packages

To install the boat's software, you must first create a catkin workspace, by following this [tutorial](http://wiki.ros.org/catkin/Tutorials/create_a_workspace). Delete you src folder and clone the boat's package as the src folder with the following command:

	$ git clone https://github.com/uwsailbot/boat_2018.git src

##Dependancies

This package relies on phidgets_imu and imu_filter_madgwick in order to compile.  Clone it from [phidgets](https://github.com/ros-drivers/phidgets_drivers) and [imu_tools](https://github.com/ccny-ros-pkg/imu_tools) (into your catkin_ws/src folder) or download both using the following command (if the following command doesn't work, just download the above git repos):

	$ rosdep install boat_nav

Either way make sure to read the README.md in their repo and follow some extra steps.

You must download the python phidgets API [See here](https://www.phidgets.com/docs/Language_-_Python#Install_Phidget_Python_module_for_Linux)

Run this in the libphidget folder to build it:

	$ ./configure --prefix=/usr && make && sudo make install

Also be sure to download the phidgets compass calibration program [See here](https://www.phidgets.com/?tier=3&catid=10&pcid=8&prodid=32)

##Finishing

You should then be able to build your catkin workspace with the command:

	$ catkin_make
