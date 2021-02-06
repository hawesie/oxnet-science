# OxNet Science Programme: Robot Navigation Data Processing 

This repository contains the data and introductory code you need for the OxNet Science Programme seminar delivered by [Prof. Nick Hawes](https://www.robots.ox.ac.uk/~nickh/) about robot navigation. If you are on the OxNet programme and have any questions about the data or code, please post your question on the [OxNet forum](https://www.oxnet.org/forum/stem-discussion-group).


## Software / Environment Setup

In order to work with this code you need to have access to [Python 3](https://www.python.org/), with the following additional packages: [numpy](https://numpy.org/) (for numerical computations, [matplotlib](https://matplotlib.org/) (for visualisation and plotting), and [scipy](https://www.scipy.org/) (used here for estimating probability densities). We will work in a [Jupyter notebook](https://jupyter.org/) for the exercise, so you also require the packages for this. 

Whilst you can install Python 3 manually, and use pip to install these packages, we recommend you use one of the two following approaches to set up your Python environment for OxNet.

### Anaconda

If you want to install Python on a laptop or desktop computer, the easiest way to get the setup you need for these exercises is to use [Anaconda](https://www.anaconda.com/products/individual). Anaconda is an app that manages your Python install and packages for you. An explanatory video for how to use Anaconda to create the correct environment for our Jupyter notebooks is available here: [https://youtu.be/x0MEaTorbtc](https://youtu.be/x0MEaTorbtc).

In that video I demonstrate how to perform the necessary setup *after* downloading and installing [Anaconda Indivual Edition](https://www.anaconda.com/products/individual), so you should do that before attempting to follow the video. In the second half of the video I download and open some Python notebooks for a different class I am teaching. You can watch this bit to understand how to open files in a notebook, but if you want to copy the steps you should use the notebook from this exercise instead.

### Amazon Web Services - SageMaker

If you do not want to, or cannot, install the software locally, then you can work with Jupyter notebooks in a free Amazon Web Services (AWS) SageMaker setup in the cloud. SageMaker Studio is the AWS-branded version of Jupyter Lab. It also comes pre-configured with all the packages we required. To access the AWS setup you  first need to apply for an AWS Educate account at the following link: [https://aws.amazon.com/education/awseducate/](https://aws.amazon.com/education/awseducate/). 

After you have been granted an account you can watch the following video for the instructions on how to set up the Python notebook environment: [https://youtu.be/6Jvsh85Q6AI](https://youtu.be/6Jvsh85Q6AI) 

In the second half of the video I upload and open some Python notebooks for a different class I am teaching. You can watch this bit to understand how to upload files to a cloud notebook, but if you want to copy the steps you should use the notebook from this exercise instead.

## Downloading the Code and Data

The Python notebook and data for this exercise is stored in this [Git repository](https://github.com/hawesie/oxnet-21-science). To download the code you can use the following link to download a zip file: [https://github.com/hawesie/oxnet-21-science/archive/main.zip](https://github.com/hawesie/oxnet-21-science/archive/main.zip). 

You should extract the file you downloaded into the location in your Python environment where you plan to work on it. This will create a folder structure containing a `data` folder and a `notebooks` folder. You should open `notebooks/robot_navigation_statistics.ipynb` in your Jupyter notebook editor. 


## Data 

The data is provided in a comma-separated value file [data/tsc_y3_nav_stats.csv](data/tsc_y3_nav_stats.csv). This file contains the navigation data from a mobile robot from the STRANDS project (a European robotics project) moving over a navigation graph structure (which we refer to a "topological map") in a office environment. For more information on the STRANDS project and the robotics technology, see the article [The STRANDS Project: Long-Term Autonomy in Everyday Environments](https://ieeexplore.ieee.org/document/7948740).

Each line in the data file describes an attempt to navigate an edge in the robot's topological map. The edge being navigated is indicated by the `edge_id`. The navigation attempt starts from the `origin` node with the aim of reaching `target`. It may successfully reach that node, or it may end up somewhere else. The place it ends up is `final_node`. Each node is a 2D point plus an *influence zone* which is an area around that point. The `time_to_waypoint` field indicates the duration (in seconds) of the navigation action until the influence zone is reached. The `operation_time` is the duration from the start of the navigation action until the action is terminated. Termination conditions may be the robot reaching the influence zone, reaching the 2D point for the node, or failing (in which case the action is cancelled by another process due to a timeout or another failure condition).

## Code

You are provided with a Jupyter notebook in [notebooks/robot_navigation_statistics.ipynb](notebooks/robot_navigation_statistics.ipynb). This notebook provides the Python code necessary to load the data and manipulate it in various ways. 

# The Homework Exercise

For the homework you should work through the provided Jupyter notebook, reading each entry and doing your best to understand each cell of Python code. Feel free to edit the code, or run additional tests, as you wish. At two locations in the file there are lists of tasks for you to attempt in order to explore the data further. Everyone should attempt at least two tasks, i.e. the first task in each list. Save all your attempts in the notebook and then you can submit your homework by submitting your edited notebook.

# Required Knowledge

In order to complete this exericse you need to have enough Python knowledge to understand, use, and extend the notebook provided. 

There are many free resources for learning Python. The one we recommend for you is this online book: http://openbookproject.net/thinkcs/python/english3e/
To prepare for this exercise we recommend trying to get through Chapters 1 to 14 (skipping 10 if you want), plus Chapter 20.

If you are particularly interested in maths and physics, you may instead want to try the introduction to Python that Oxford and Cambridge provide for their undergraduate engineers: https://github.com/hawesie/a2-computer-engineering/

The exercise also requiures knowledge about data handing and visualisation, statistics (mean, standard deviation), and probability.


