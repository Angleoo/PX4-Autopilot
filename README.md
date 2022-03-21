# PX4-Autopilot

Git clone default PX4-Autopilot
```
git clone https://github.com/PX4/PX4-Autopilot.git --recursive
bash ./PX4-Autopilot/Tools/setup/ubuntu.sh
```

1) Copy s500 folder to ./PX4-Autopilot/Tools/sitl_gazebo/models
2) Move emptyworld.world to ./PX4-Autopilot/Tools/sitl_gazebo/worlds
3) Replace the sitl_target.cmake file at ./PX4-Autopilot/platforms/posix/cmake

Run PX4-Autopilot SITL & Gazebo
```
cd ./PX4-Autopilot
make px4_sitl gazebo_s500__emptyworld
```

# Insall QGroundControl

Add current user accout to dialout group and remove modemmanager
```
sudo usermod -a -G dialout $USER
sudo apt-get remove modemmanager
```

Download QGroundControl.AppImage 
```
wget https://s3-us-west-2.amazonaws.com/qgroundcontrol/latest/QGroundControl.AppImage
```
Change permissions and run 
```
chmod +x ./QGroundControl.AppImage 
./QGroundControl.AppImage
```
