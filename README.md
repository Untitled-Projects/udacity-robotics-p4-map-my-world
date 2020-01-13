Udacity Robotics Software Engineer Nanodegree Project 4 Map My World by Michael Strobl

1- Add Teleop Twist Keyboard 

    $ cd ~/catkin_ws/src
    $ git clone https://github.com/ros-teleop/teleop_twist_keyboard


2- Build the project:
    
    $ cd ~/catkin_ws
    $ catkin_make


3- Launch the robot inside your world

    $ cd ~/catkin_ws
    $ source devel/setup.bash
    $ roslaunch my_robot world.launch\

4- Use teleop_twist_keyboard for navigation (in a new terminal)

    $ cd ~/catkin_ws
    $ source devel/setup.bash
    $ rosrun teleop_twist_keyboard teleop_twist_keyboard.py


5- Launch Mapping file (in a new terminal)

    $ cd ~/catkin_ws
    $ source devel/setup.bash
    $ roslaunch my_robot mapping.launch

Drive around to map the world and close the terminal to save the map.


Note: to change the directory of the saved map you need to change the mapping.launch file (~/catkin_ws/src/my_robot/launch) under the argument “database_path”.

6- View Map

    $ rtabmap-databaseViewer ~/.ros/rtabmap.db


Sources:

- Udacity Robotics Software Engineer Nanodegree Project 4

Link to Map:
- https://drive.google.com/open?id=1c_ZmhUHSx29xmv2DfY6shdrz-vV-NPkv