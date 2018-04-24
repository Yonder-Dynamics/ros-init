robot_upstart is used to autostart the launch file  
The raspberry pi requires the motor driver, which is currently procyon-motor-ctl.  
The raspberry pi automatically launches a motor driver that listens to MotorCMD messages.  

rosrun robot_upstart install ros_init/launch/rpi.launch  
sudo systemctl start ros  
  
check logs:  
sudo tail /var/log/upstart/myrobot.log -n 30  
