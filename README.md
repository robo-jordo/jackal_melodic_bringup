# jackal_melodic_bringup

---

This README contains instructions of bringing up the [Clearpath Jackal](https://clearpathrobotics.com/jackal-small-unmanned-ground-vehicle/) on a new version of ROS before official support from Clearpath.
In this case this was done for [ROS melodic](http://wiki.ros.org/melodic) in October 2019.

**Note:** This also includes isntructions and code for bringing up the jackal with a velodyne 3D lidar, the lidar specific steps can be omitted for jackals without the lidar, These steps will be marked with ???

![alt text](https://www.unmannedsystemstechnology.com/wp-content/uploads/2014/09/Jackal-UGV.jpg)

---

## Fresh start
In order to bring up the jackal with ROS melodic I reccomend using a new SSD and not wiping your old SSD, this may be helpful if you make a mistake and want to backtrack to a working state for your system. I also found this helpful for debugging things like udev rules that were correctly configured by clearpath but are not documented.

#### 1. steps to a fresh Ubuntu 18.04 start:
   * Prepare a bootable USB with an Ubuntu 18.04 image. Following the [Official Ubuntu instructions for booting from USB](https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-ubuntu#0) is recommended.

   * While the Jackal is powered off, insert the bootable USB into the Jackal along with a keyboard, mouse and monitor.

   * The Jackal should automatically boot with the USB (If it does not then hold F12 while booting)

   * The [official Ubuntu installation instructions](https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop#3) will help you through the process if necessary.

   * Once complete, remove the bootable USB and restart the Jackal. It should start up with your regular Ubuntu login screen

#### 2. Setting up wireless networking:
   (This step is not strictly speaking necessary but being able to connect to the Jackal over WiFi is far more convenient.)

   *
