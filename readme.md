idek

how to run
```bash
ros2 launch lunch.py
```

generate map from .world file:
```bash
ros2 launch slam_toolbox online_async_launch.py use_sim_time:=true
```

in new terminal 
```bash
ros2 run turtlebot3_teleop teleop_keyboard
```
and navigatge through gazebo; go around the map

save the map with 
```bash
ros2 run nav2_map_server map_saver_cli -f ~/FILE_NAME
```

replace FILE_NAME with <map> in lunch.py



