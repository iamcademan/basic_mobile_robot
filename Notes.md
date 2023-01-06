# Initial Install/Build

## Dependencies

sudo apt install ros-humble-navigation2
sudo apt install ros-humble-nav2-bringup
sudo apt install ros-humble-joint-state-publisher-gui
sudo apt install ros-humble-xacro
sudo apt-get install gedit

## Run the following to setup environment

```echo "source /usr/share/colcon_cd/function/colcon_cd.sh" >> ~/.bashrc echo "export _colcon_cd_root=~/dev_ws" >> ~/.bashrc```

## To create the base package

In a terminal copy and paste each cmd and press enter:
ros2 pkg create --build-type ament_cmake basic_mobile_robot
cd ~/dev_ws/src/basic_mobile_robot
mkdir config launch maps meshes models params rviz worlds

## Initial Build:

cd ~/dev_ws
colcon build --packages-select basic_mobile_robot

# Building:

cd ~/dev_ws
colcon build --packages-select basic_mobile_robot --symlink-install

# Basic Launching

```cd ~/dev_ws/```

```source ~/dev_ws/install/setup.bash ros2 launch basic_mobile_robot basic_mobile_bot_v1.launch.py```

TO SEE PARAMS:

```ros2 launch -s basic_mobile_robot basic_mobile_bot_v1.launch.py```

# References:

* [https://automaticaddison.com/how-to-create-a-simulated-mobile-robot-in-ros-2-using-urdf/](https://)
* [https://automaticaddison.com/set-up-the-odometry-for-a-simulated-mobile-robot-in-ros-2/](https://)

```

```
