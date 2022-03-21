# PX4-Autopilot


1) git clone https://github.com/PX4/PX4-Autopilot.git --recursive
2) bash ./PX4-Autopilot/Tools/setup/ubuntu.sh

3) Copy s500 folder to ./PX4-Autopilot/Tools/sitl_gazebo/models
4) Move emptyworld.world to ./PX4-Autopilot/Tools/sitl_gazebo/worlds
5) Replace the sitl_target.cmake file at ./PX4-Autopilot/platforms/posix/cmake

6) cd ./PX4-Autopilot
7) make px4_sitl gazebo_s500__emptyworld
