Steps install ros in ubuntu

Installation

Configure your Ubuntu repositories: sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

Set up your keys

sudo apt install curl # if you haven't already installed curl curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

Installation: sudo apt update

**Desktop-Full Install: (Recommended) ** sudo apt install ros-noetic-desktop-full

Desktop Install: Everything in ROS-Base plus tools like rqt and rviz sudo apt install ros-noetic-desktop

ROS-Base: (Bare Bones) ROS packaging, build, and communication libraries. No GUI tools. sudo apt install ros-noetic-ros-base

** more packages available in ROS.** sudo apt install ros-noetic-PACKAGE sudo apt install ros-noetic-slam-gmapping

Environment setup echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc source ~/.bashrc

zsh: echo "source /opt/ros/noetic/setup.zsh" >> ~/.zshrc source ~/.zshrc

Dependencies for building packages sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

Initialize rosdep sudo apt install python3-rosdep

here initialize rosdep.

sudo rosdep init rosdep update
