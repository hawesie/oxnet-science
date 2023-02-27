
# Getting Help

If you get stuck with any of this, or just have questions, please get in touch with Thomas Hird <thomas.hird@physics.ox.ac.uk> or use one of the other OxNet channels.

# Preparing Your Coding Environment

## Setting up the Cloud Python Environment

In this course we will do all our Python programming in a [Jupyter notebook environment](https://jupyter.org). A notebook is a web-based interactive computing platform — in short, this allows you to write Python code in your browser, and also write notes and explanations alongside it (that’s the “interactive” part). You should already have an [AWS SageMaker Studio Lab](https://studiolab.sagemaker.aws) (SSL) account to provide the notebook environment. 

**IMPORTANT**: Your SSL runtime really is running a (virtual) computer somewhere in the AWS cloud. This means that even when you’re not using it, it’s using resources such as electricity and generating heat. To avoid wasting the planet’s resources (and AWS’s money), you must remember to stop the runtime when you’ve finished your coding session. If you leave it running without, you may find find that AWS lock your account.

### I’m new to Jupyter Notebooks!

If you are new to Jupyter notebooks, the best way to learn about them is to use them! Before you dive right in though, it may be worth watching or reading a quick tutorial on the basics of working with them. The following links give some tutorial material you may find useful. Note that you can **ignore material on installing and starting Jupyter** since SageMaker Studio Lab (described above) is how you will access our chosen version of Jupyter lab. 

Links for learning about Jupyter notebooks (remember, your installation/running part is with SageMaker Studio)

- Youtube Videos
    - Jupyter Notebook Tutorial [https://youtu.be/DKiI6NfSIe8](https://youtu.be/DKiI6NfSIe8)
    - Jupyter Notebook Tutorial for Beginners with Python: [https://youtu.be/2WL-XTl2QYI](https://youtu.be/2WL-XTl2QYI)
- Web pages:
    - [https://realpython.com/jupyter-notebook-introduction/](https://realpython.com/jupyter-notebook-introduction/)
    - [https://www.dataquest.io/blog/jupyter-notebook-tutorial/](https://www.dataquest.io/blog/jupyter-notebook-tutorial/) (goes into data science later, which you can ignore)

## Preparing for Python

You should already be familiar with programming in Python from the study day and initial material provided by OxNet. If you missed this, or still do not feel confident enough with Python to complete the exercise, please see the "Getting Help" section above.

# OxNet Science Homework 1

To get started with the homework, follow the steps below:

1. Log on to SageMaker Studio Lab, start the runtime, and open your project.
2. Open the “Git” mention and select “Clone Git Repository”
3. This will pop up a dialogue box. In the empty field (”Git repository URL (.git):”) paste the following: [https://github.com/hawesie/oxnet-science.git](https://github.com/hawesie/oxnet-science.git)
4. Uncheck the box after “Search for environment.yml and build Conda environment.” (but leave the other one checked).
5. Click the blue Clone button

This will copy the Python activity files into your project and open this README file. 

You can then open the file for the homework and get started: [notebooks/robot_navigation_statistics.ipynb][notebooks/robot_navigation_statistics.ipynb]

