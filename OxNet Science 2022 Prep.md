# OxNet Science 2022

Welcome to the OxNet Science programme for 2022. In this course you will learn how scientists from a range of disciplines use mathematical models to understand phenomena in their fields, and get hands-on experience building and applying these models using the programming language Python. 

During the six seminars you will be taught the necessary maths to understand the models that we will cover, and the Python exercises will be structured so that you do not need to be a programming expert to learn from them. However, we have found that you will get the most benefit from this course if you have some experience with Python before you start the seminars. Therefore this document aims to get you started with the necessary Python tools and some basic programming. Please read it all carefully, and follow the instructions provided.

# Getting Help

If you get stuck with any of this, or just have questions, please get in touch with Holly Roach <[holly.roach@path.ox.ac.uk](mailto:Holly%20Roach%20%3Cholly.roach%40path.ox.ac.uk%3E)>, or post in the OxNet forum.

# Preparing Your Coding Environment

## Setting up the Cloud Python Environment

In this course we will do all our Python programming in a [Jupyter notebook environment](https://jupyter.org). A notebook is a web-based interactive computing platform — in short, this allows you to write Python code in your browser, and also write notes and explanations alongside it (that’s the “interactive” part). Whilst you can install Python and the Jupyter notebook framework on a computer, we have found it is much easier for students to work in a cloud environment. This means you can write and run code from any web browser, with no local installation required.

We will use [AWS SageMaker Studio Lab](https://studiolab.sagemaker.aws) (SSL) as the cloud provider. Therefore the first thing you should do is go to the SSL site and request a new account. The link to follow to do this is: [https://studiolab.sagemaker.aws/requestAccount](https://studiolab.sagemaker.aws/requestAccount) 

When requesting the account please use your own details (name, email etc.), but use “Pembroke OxNet Science” when you are asked for a company or organisation name.

After requesting an account it may take a few days to get a response, so make sure you request an account sooner rather than later (don’t leave it until the last minute). 

SageMaker Studio Lab creates a “runtime” in the cloud for you. This runtime is simply a virtual computer that will host your Python code. Once you have your account, sign in then select “CPU” for the compute type, and press “Start runtime”.  The page will spend a little time saying “Preparing project runtime...” then it will be ready. Once it is ready you can click the “Open project” this will take you to a page titled “Getting Started with Amazon SageMaker Studio Lab”. Feel free to read the first few paragraphs to understand how to interact with the notebook.

**IMPORTANT**: Your runtime really is running a (virtual) computer somewhere in the AWS cloud. This means that even when you’re not using it, it’s using resources such as electricity and generating heat. To avoid wasting the planet’s resources (and AWS’s money), you must remember to stop the runtime when you’ve finished your coding session. If you leave it running without, you may find find that AWS lock your account.

### I’m new to Jupyter Notebooks!

I expect most of you will be new to Jupyter notebooks. As with most things related to programming, the best way to learn about them is to use them! Before you dive right in though, it may be worth watching or reading a quick tutorial on the basics of working with them. The following links give some tutorial material you may find useful. Note that you can **ignore material on installing and starting Jupyter** since SageMaker Studio Lab (described above) is how you will access our chosen version of Jupyter lab. 

Links for learning about Jupyter notebooks (remember, your installation/running part is with SageMaker Studio)

- Youtube Videos
    - Jupyter Notebook Tutorial [https://youtu.be/DKiI6NfSIe8](https://youtu.be/DKiI6NfSIe8)
    - Jupyter Notebook Tutorial for Beginners with Python: [https://youtu.be/2WL-XTl2QYI](https://youtu.be/2WL-XTl2QYI)
- Web pages:
    - [https://realpython.com/jupyter-notebook-introduction/](https://realpython.com/jupyter-notebook-introduction/)
    - [https://www.dataquest.io/blog/jupyter-notebook-tutorial/](https://www.dataquest.io/blog/jupyter-notebook-tutorial/) (goes into data science later, which you can ignore)

## Preparing for Python

Once you have your Jupyter environment up and running, what you do next depends on your level of previous programming experience. 

### I’ve never programmed before/I hate programming!

If you have never done *any* programming before, or are someone who finds programming  challenging, then you may find that the practical parts of this course are quite hard to access. Please do not worry about this, and do talk to us if you are struggling. To get the most out of the activities, it is definitely worth spending some time now learning Python. As a starting point we highly recommend working slowly through the textbook [How to Think Like a Computer Scientist: Learning with Python 3](https://openbookproject.net/thinkcs/python/english3e/) (click the link to access the book). This book covers the key aspects of programming in Python from the very basics, and builds up to everything you need to know in this course.  In particular you should work through Chapters 1 to 14 (skipping 10 if you want), plus Chapter 20. If you get this far, then you could tackle the provided Python activity (see [below](https://www.notion.so/OxNet-Science-2022-45d4d1172074451ca17d54dab2cce63a)) to test yourself.

### I’ve programmed before but I’m new to Python

If you have learned another language (e.g. Java, C++, Javascript, R) but not Python, then you will need to pick up the **syntax** of python (i.e. what symbols to type in what order). The provided Python activities (see [below](https://www.notion.so/OxNet-Science-2022-45d4d1172074451ca17d54dab2cce63a)) should provide you with enough scope to learn the way Python works, and help you translate your experience from other languages.

### I’ve got some experience with Python

If you have worked with Python before, it will be useful to make sure you revise all the topics and libraries relevant to this course.  The provided Python activities (see [below](https://www.notion.so/OxNet-Science-2022-45d4d1172074451ca17d54dab2cce63a)) will help your revision. If you want to revise independently then make sure you cover list processing, dictionaries, numerical computing with `numpy` and visualisations using `matplotlib`.

## OxNet Python Prep Activities

As mentioned above, we have provided some Python exercises to make sure you’re up to speed by the time the OxNet seminars start. Once you have got your SSL account set up (see above), you should do the following:

1. Log on to SageMaker Studio Lab, start the runtime, and open your project.
2. Open the “Git” mention and select “Clone Git Repository”
3. This will pop up a dialogue box. In the empty field (”Git repository URL (.git):”) paste the following: [https://github.com/hawesie/oxnet-python-prep](https://github.com/hawesie/oxnet-python-prep)
4. Uncheck the box after “Search for environment.yml and build Conda environment.” (but leave the other one checked).
5. Click the blue Clone button

This will copy the Python activity files into your project and open the README file. You should read this and then get started on the exercises.

These steps are illustrated in a video, here: [https://youtu.be/qgy7XWhXT6o](https://youtu.be/qgy7XWhXT6o)

# What’s Next?

Once you are able to run a SageMaker Studio Lab project, are able to work with a Jupyter notebook, and are comfortable with Python, then you’re ready to go! The next step will be the first session where we’re looking a mathematical models in probability theory and robotics.