# Udacity Nanodegree - Robotics Software Engineer - Project3

This is my project submission for Project4: Map My World of [Udacity Nanodegree - Robotics Software Engineer](https://www.udacity.com/course/robotics-software-engineer--nd209?irclickid=U9u1PgV1xxyIROOV3m3wlTMuUkD0yqTMORvH3A0&irgwc=1&utm_source=affiliate&utm_medium=&aff=2298976&utm_term=&utm_campaign=__&utm_content=&adid=786224).

## Requirements
1. Git clone this workspace or clone the my_robot package into your workspace.
2. Git clone https://github.com/ros-teleop/teleop_twist_keyboard into the workspace `src` folder
3. Install [rtabmap_ros](https://github.com/introlab/rtabmap_ros)
4. Downlaod the rtabmap.db file from [here](https://drive.google.com/file/d/1Rg4rg72OJPalNaf11qqLJVfczxzUEsHs/view?usp=sharing) and place it in my_robot/maps/ folder.
5. `catkin_make` the workspace

## Usage
1. Source the workspace and roslaunch the world.launch:
    ```
    source devel/setup.bash
    roslaunch my_robot world.launch
    ```
2. Open another terminal and roslaunch the localization.launch. (remember to source the workspace again)
    ```
    roslaunch my_robot localization.launch
    ```
3. Open a new terminal and launch the teleop.launch (remember to source the workspace again)
    ```
    roslaunch my_robot teleop.launch
    ```
4. You should be able to see the map stored in my_robot/maps/rtabmap.db is used and displayed on rviz.

5. Navigate the robot around and the robot will be able to localize itself.

6. If you would like to redo a new map:
    ```
    roslaunch my_robot mapping.launch
    ```

## Screenshots
![Screenshot01](https://github.com/tka-andrew/RoboND-Project3/blob/master/Screenshots/screenshot01.png?raw=true)