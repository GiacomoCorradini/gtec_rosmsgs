The original repository is: https://github.com/GTEC-UDC/rosmsgs, some changes have been made in order to be able to compile it for [ROS2 Humble](https://docs.ros.org/en/humble/index.html)

# OLD README

**NOTE:** This repository is related with the next scientific work:

**Barral, V.**; **Escudero, C.J.**; **García-Naya, J.A.**; **Maneiro-Catoira, R.** *NLOS Identification and Mitigation Using Low-Cost UWB Devices.* Sensors 2019, 19, 3464.[https://doi.org/10.3390/s19163464](https://doi.org/10.3390/s19163464)

If you use this code for your scientific activities, a citation is appreciated.

## README

Update version in order to be used in ros2 environment

This project contains a set of custom ROS message definitions used in several GTEC ROS nodes.

* ```msgs::Ranging``` This message models a range value between a tag and a anchor.
* ```msgs::PozyxRanging``` This message models a range value between a tag and an anchor from a Pozyx tag/anchor. It encapsulates some of the parameters provided by the DW1000, like ranging values and quality measurements.
* ```msgs::DWRanging``` This message models a range value between a tag and an anchor from a EBV1000 tag/anchor.

## Compile the project

```cmake
colcon build
```

To use the messages the source is needed:

```sh
source install/setup.bash
```