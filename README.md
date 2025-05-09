# rt2_assignment2
### This repository is for assignment 2 in Research Track 2

This project is a Jupyter Notebook implementation for controlling a robot and visualizing its state in real time.

The notebook includes:

- An interface to assign or cancel goals to the robot  
- Display of the current distance to the closest obstacle  
- A plot showing the robot's trajectory 
- A plot showing the number of reached and not-reached targets

## How to run
**Step 1: Build the Package**

 1. First, you need to clone the `assignment_2_2024` repository in your workspace:
 https://github.com/CarmineD8/assignment_2_2024
 2. In addition, you need to clone the `rt_assignment2_part1` repository into the same workspace:
 https://github.com/yuimomi/rt_assignment2_part1.git

3. Then, compile the workspace with:
    ```bash
    cd ~/catkin_ws
    catkin_make
    source devel/setup.bash
    ```
**Step 2: Launch the Nodes**

1. First, launch the simlation environment with:
    ```bash
    roslaunch assignment_2_2024 assignment1.launch 
    ```
2. Then, launch service node.
    ```bash
    roslaunch my_assignment2 my_assignment2.launch use_jupyter:=true
    ```

3. In the notebook, start the action node by restarting the kernel and run all the cells.

**Step 3: Interact with the System**
1. Use the input fields to assign goals to the robot.
2. Observe the robot's trajectory and progress in the plots.
3. The number of reached and not-reached targets will update automatically.

## Requirements

- Jupyter Notebook
- matplotlib
- ipywidgets

