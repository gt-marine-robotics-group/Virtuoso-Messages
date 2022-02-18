# Virtuoso-Messages
ROS2 workspace for mapping custom messages used by Virtuoso from ROS1 to ROS2. 

To run the mappings with ros1_bridge:
1. Make sure ros1_bridge has been built from source (i.e. clone it into a separate workspace and run `colcon build packages-select ros1_bridge --cmake-force-configure`).
2. Source ros1
3. Source ros2
4. Source vrx workspaces containing the custom messages
5. Source Virtuoso-Messages
6. Source ros1_bridge
7. `ros2 run ros1_bridge dynamic_bridge --bridge-all-topics`
