# jackal_melodic_bringup

This README contains instructions of bringing up the [Clearpath Jackal](https://clearpathrobotics.com/jackal-small-unmanned-ground-vehicle/) on a new version of ROS before official support from Clearpath.
In this case this was done for [ROS melodic](http://wiki.ros.org/melodic) in October 2019.

**Note:** This also includes isntructions and code for bringing up the jackal with a velodyne 3D lidar, the lidar specific steps can be omitted for jackals without the lidar, These steps will be marked with ???

![alt text](https://www.google.com/url?sa=i&source=images&cd=&ved=2ahUKEwiXxse1prPlAhWOr54KHVJoBg8QjRx6BAgBEAQ&url=https%3A%2F%2Fclearpathrobotics.com%2Fjackal-small-unmanned-ground-vehicle%2F&psig=AOvVaw1Icin28CcguF29lsWiPmAc&ust=1571951662190660)

## Fresh start
In order to bring up the jackal with ROS melodic I reccomend using a new SSD and not wiping your old SSD, this may be helpful if you make a mistake and want to backtrack to a working state for your system. I also found this helpful for debugging things like udev rules that were correctly configured by clearpath but are not documented.

steps to a fresh Ubuntu 18.04 start:
* Prepare a bootable USB with an Ubuntu 18.04 image. Following the [Official Ubuntu instructions for booting from USB](https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-ubuntu#0) is recommended.