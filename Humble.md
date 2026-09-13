
```bash
# /etc/systemd/system/rover-bringup.service
[Unit]
Description=Rover ROS 2 bringup
After=network.target

[Service]
Type=simple
User=rover
ExecStart=/bin/bash -c 'source /opt/ros/humble/setup.bash && source /home/rover/mars_rover_ws/install/setup.bash && ros2 launch rover_bringup bringup.launch.py'
Restart=on-failure
RestartSec=3

[Install]
WantedBy=multi-user.target
```
