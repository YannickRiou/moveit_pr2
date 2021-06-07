moveit_pr2
==========

MoveIt! Packages for PR2 which contains SRDF files with pre-defined poses, planning groups but also planner configuration and move_group launch files.

## To launch in demo/simulation (without the robot)

`
roslaunch pr2_moveit_config demo.launch 
`

It will launch the move_group node, load the robot description and a fake joint_state_publisher. Rviz will also open to be able to control the robot directly.

## To launch when working on the real robot

To launch the move_group node : 
`
roslaunch pr2_moveit_config pr2_moveit.launch 
`
If you want to enable octomap, just set the following parameter to true : 

`
roslaunch pr2_moveit_config pr2_moveit.launch use_octomap:=true
`

To launch rviz : 
`
roslaunch pr2_moveit_config moveit_rviz.launch
`

## To launch the moveit setup assistant 

`
roslaunch pr2_moveit_config setup_assistant.launch
`
