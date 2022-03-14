# OxNet Science Programme: Robot Navigation Data Processing 

This is the README file for the OxNet Science Programme seminar delivered by [Prof. Nick Hawes](https://www.robots.ox.ac.uk/~nickh/) about robot navigation. If you are on the OxNet programme and have any questions about the data or code, please post your question on the [OxNet forum](https://www.oxnet.org/forum/stem-discussion-group) or get in touch with Holly Roach <[holly.roach@path.ox.ac.uk](mailto:Holly%20Roach%20%3Cholly.roach%40path.ox.ac.uk%3E)>.


## Software / Environment Setup

In order to prepare your computing environment, make sure you've completed "Preparing Your Coding Environment" from the [README.md](./README.md). If you are not following those instructions for some reason, then in order to work with this code you need to have access to [Python 3](https://www.python.org/), with the following additional packages: [numpy](https://numpy.org/) (for numerical computations) and [matplotlib](https://matplotlib.org/) (for visualisation and plotting). We will work in a [Jupyter notebook](https://jupyter.org/) for the exercise, so you also require the packages for this. 


## Downloading the Code and Data

The Python notebook and data for this exercise is stored in this [Git repository](https://github.com/hawesie/oxnet-science). To use the code in SageMaker, do the following

1. Log on to SageMaker Studio Lab, start the runtime, and open your project.
2. Open the “Git” mention and select “Clone Git Repository”
3. This will pop up a dialogue box. In the empty field (”Git repository URL (.git):”) paste the following: [https://github.com/hawesie/oxnet-science](https://github.com/hawesie/oxnet-science)
4. Uncheck the box after “Search for environment.yml and build Conda environment.” (but leave the other one checked).
5. Click the blue Clone button

This should extract the files into your Python environment. It will create a folder structure containing a `data` folder and a `notebooks` folder. You should open `notebooks/robot_navigation_statistics.ipynb` in SageMaker Studio Lab.


## Data 

The data is provided in a comma-separated value file [data/tsc_y3_nav_stats.csv](data/tsc_y3_nav_stats.csv). This file contains the navigation data from a mobile robot from the STRANDS project (a European robotics project) moving over a navigation graph structure (which we refer to a "topological map") in a office environment. For more information on the STRANDS project and the robotics technology, see the article [The STRANDS Project: Long-Term Autonomy in Everyday Environments](https://ieeexplore.ieee.org/document/7948740).

Each line in the data file describes an attempt to navigate an edge in the robot's topological map. The edge being navigated is indicated by the `edge_id`. This is indicated by the `edge_id`. The navigation attempt starts from the `origin` node with the aim of reaching `target`. It may successfully reach that node, or it may end up somewhere else. The place it ends up is `final_node`. Each node is a 2D point plus an *influence zone* which is an area around that point. The `operation_time` field indicates the duration (in seconds) of the navigation action until the influence zone is reached. The `time_to_waypoint` is the time spend in the navigation action after the influence zone is reached until the action is terminated. Termination conditions may be the robot reaching the 2D waypoint for the node, having a new action superseding the current one, or failing (in which case the action is cancelled by another process due to a timeout or another failure condition). These durations can be matched to the dates as follows, `operation_time = date_finished - date_started`, `time_to_waypoint = date_finished - date_at_node` but they were  recorded with sub-second accuracy.

## Code

You are provided with a Jupyter notebook in [notebooks/robot_navigation_statistics.ipynb](notebooks/robot_navigation_statistics.ipynb). This notebook provides the Python code necessary to load the data and manipulate it in various ways. 

# The Homework Exercise

For the homework you should work through the provided Jupyter notebook, reading each entry and doing your best to understand each cell of Python code. Feel free to edit the code, or run additional tests, as you wish. At two locations in the file there are lists of tasks for you to attempt in order to explore the data further. Everyone should attempt at least two tasks, i.e. the first task in each list. Save all your attempts in either the provided notebook or a separate one, and then you can submit your homework by submitting your edited notebook.

