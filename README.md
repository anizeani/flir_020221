









































































































































Prerequisites
######
1. ROS kinetic installed
2. catkin tools installed
3. rosdep is installed
4. apt update was done recently
5. rosdep update was done recently

INSTALL
######

1. Create folder (f.e. flir_tools_ws)
2. source /opt/ros/kinetic/setup.bash
3. Create folder flir_tools_ws/src
4. Inside flir_tools_ws: catkin init
5. Inside flir_tools_ws/src : git clone URLHERE .
6. sudo apt update
7. rosdep update
8. Inside flir_tools_ws: rosdep install --from-paths src --ignore-src --rosdistro kinetic -r 
9. Inside flir_tools_ws: catkin build

Usage
######
1. source flir_tools_ws/devel/setup.bash
2. roslaunch ir_rgb_extractor extract_falsecolor_ir_and_rgb.launch ir_topic:="/ir_topic/from/rosbag" ir_folder:="/path/to/save/ir/pictures" rgb_topic:="/rgb_topic/from/rosbag" rgb_folder:="/path/to/save/rgb/pictures" rosbag_file:="/path/to/rosbag.bag"