# eces373_f22_aas220_navvis_description
First pull the code from the git repo
run catkin_make, then source your setup.bash
Command for roslaunch withuot xacro run from the src is roslaunch navvis_description/launch/display.launch
Command for roslaunch with xacro is roslaunch navvis_description/launch/display.launch use_xacro:=true
Command to run the joint state publisher rosrun joint_state_publisher_gui joint_state_publisher_gui &

rostopic pub -1 /joint_states sensor_msgs/JointState "header:
seq: 1
stamp: {secs: 1, nsecs: 0}
frame_id: 'base'
name: ['base_wheel_left_joint', 'base_wheel_right_joint']
position: [0.0, 0.0]
velocity: [0, 0]
effort: [0, 0]" 
