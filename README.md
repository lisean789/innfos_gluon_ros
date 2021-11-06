innfos gluon ros controlled by spacenav

This packages is to enable INNFOS gluon to be controlled by a 3Dconnexon spacenav.

This package is a modification based on:
https://github.com/innfos/ros_gluon

Dependicies in it must be installed. I have changed its hardware interface a bit, so you can start launching the arm in any joint position. However, you have to have every joint encoder correctly configured beforehand. Use the INNFOS Actuator Studio to to set LPH on and correctly home the 0 of each joint.


Additinoal dependency:

sudo apt install spacenavd
sudo apt install ros-melodic-spacenav-node


You could change the moveit servo settings in this path:
/gluon_control/config/gluon_spacenav_config.yaml


Launch:
Simply launch the following with the gluon in any position.

roslaunch gluon_control control_by_spacenav.launch


I've been looking for people who owns a gluon to play it together!

