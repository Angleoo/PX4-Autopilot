# PX4-Autopilot


git clone https://github.com/PX4/PX4-Autopilot.git --recursive
bash ./PX4-Autopilot/Tools/setup/ubuntu.sh

Copy s500 folder to ./PX4-Autopilot/Tools/sitl_gazebo/models
Move emptyworld.world to ./PX4-Autopilot/Tools/sitl_gazebo/worlds
Replace the sitl_target.cmake file at ./PX4-Autopilot/platforms/posix/cmake

cd ./PX4-Autopilot
make px4_sitl gazebo_s500__emptyworld
