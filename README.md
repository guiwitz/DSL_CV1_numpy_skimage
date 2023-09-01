# Data Science Lab Computer Vision course with Python
## 1. Basics with numpy and scikit-image

This course covers the basics of Computer Vision with Python via a series of Jupyter notebooks. Those rusty with Python can have a look at the [01-python_basics](01-python_basics) content which briefly summarizes the essentials of the language needed for the course. Then the content of [02-basics_image_handling](01-basics_image_handling) mainly covers the handling of numpy arrays, which are the essential data structure used for images in Python. The [03-basic_image_processing](03-basic_image_processing) part then covers classical computer vision operations such as filtering, intensity-based segmentation, object measurement. And finally the [04-special_topics](04-special_topics) covers basics of various common workflows such as registration or tracking.

The goal of this course is not to be an exhaustive Computer Vision course and contains very little theoretical information. The goal is rather to give participants the necessary background on the tools they might want to use later for their own Computer Vision projects.

## Getting the material

To use all notebooks locally, you can simply clone (if you know git) or download the repository by using the green "Code" button at the top right of the repository. Place the folder in easily reachable location on your computer.

You can download all necessary data from [this link](). Place the main data folder then in the main folder of the downloaded repository for paths to be correct.

## Setting up an environment

A series of packages is necessary to run the content of this notebook. We highly recommend to install packages within an environment such as provided by conda. There are multiple ways to install conda and if you don't yet have a version installed we strongly recommend to use mambaforge which will install the fast environment solver mamba. You can find installers at [this link](https://github.com/conda-forge/miniforge#mambaforge).

Once you have conda/mamba installed, open a terminal where you have access to conda (i.e. the beginning of the line on your terminal window should indicate ```(base)```). On MacOS or Linux, your regular terminal should work. On Windows, depending how you installed conda, you might only have access to it from a terminal called XXX Prompt where XXX stands for Anaconda, Miniforge etc. depending how conda was installed.

Then in that terminal head to the folder of the repository you downloaded previously. In the main folder you will find an [environment.yml](environment.yml) file that contains infos about all packages to install. You can simply create the necessary environment using:

    mamba env create -f environment.yml

if you have mamba installed or

    conda env create -f environment.yml

This creates an environment called ```dslskimage``` that you then need to activate (here mamba or conda doesn't matter):

    conda activate dslskimage

Finally you can start Jupyterlab using:

    jupyter lab

This should automatically open a Jupyterlab session in your favorite browser. If not, copy the address appearing in the terminal starting with ```http://localhost:8888...``` in your browser.

## Google Colab

If installation fails or isn't working properly, a fallback solution is to use Google's version of Jupyter called Colab. You can open the notebooks of this course using this button: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/DSL_CV1_numpy_skimage/blob/colab). Most packages come pre-installed and missing ones can be installed "on the fly" in each notebook.

## Authors

Guillaume Witz, Data Science Lab, University of Bern