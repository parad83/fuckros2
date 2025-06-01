idek

how to run
```bash
ros2 launch lunch.py
```

---
### generate new map (im using simple mock)

generate map from .world file (include model: `<uri>model://turtlebot3_burger</uri>`)
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

---

problesm:
too many
- global state error in rviz
- cant set the init pos in rviz EVEN THOUGH ACML SEES IT; probably wrong nav2 params file no idea how to set it up
