# XBOX ONE ROS JOY TELEOP

## This is node for teleop robot with ros 

## Install 



```
sudo apt install -y ros-<distro>-joy
sudo git clone https://github.com/paroj/xpad.git /usr/src/xpad-0.4
sudo dkms install -m xpad -v 0.4
```

Then connect joy via nano reciver and !!!`DirectInput Mode`!!! (`D` letter at the front of pad).

To test if joy works use `jstest /dev/input/js{0}`


## Usage

```
rosrun joy joy_node
rosrun logitech_f710_joy_ros f710_teleop_joy
```

OR

```
roslaunch logitech_f710_joy_ros joy_teleop.launch
```

Move robot:

Move `X` direction and rotate `Th` left axis.

Move in Y direction right axis. 

Parking mode hold `LB` Key.

Turbo hold `RB` key.