Webstep 2019 Scikit-learn Tutorial
================================

This tutorial is intended for developers, data analysts, and related technical developers who are familiar with the Python programming language and want to learn the basics of Machine Learning with scikit-learn. By the end of this tutorial, you will be equipped with the core skills required to work with data and properly build Machine Learning models for real-world problems.

Based on the [SciPy 2018 tutorial](https://github.com/amueller/scipy-2018-sklearn) by [Kyle Kastner](https://kastnerkyle.github.io/), [Sebastian Raschka](http://sebastianraschka.com), [Andreas Mueller](http://amueller.github.io), and [others](https://github.com/amueller/scipy-2018-sklearn/graphs/contributors).

Instructors
-----------

- [Dr. Randy Olson](http://randalolson.com)  [(@randal_olson)](https://twitter.com/randal_olson) - Lead Data Scientist at [Life Epigenetics](http://lifeegx.com)

---


This repository will contain the teaching material and other information associated with our scikit-learn tutorial.

Parts 1 to 12 make up the day 1 session, while
parts 13 to 23 will be presented in the day 2 session.

### Schedule:

The 2-part tutorial will be held on Saturday and Sunday, 19-20 October, 2019.

- Parts 1 to 12: 19 October, 09.00 - 17.00
- Parts 13 to 23: 20 October, 09.00 - 15.00


### Backchannel:

Please feel free to use this channel to share answers and ask questions: https://etherpad.net/p/webstep-ml-2019



Obtaining the Tutorial Material
--------------------------------

If you have a GitHub account, it is probably most convenient if you clone or
fork the GitHub repository. You can clone the repository by running:

```bash
git clone https://github.com/rhiever/webstep-sklearn-quickstart-2019.git
```

 If you are not familiar with git or don’t have an
GitHub account, you can download the repository as a .zip file by heading over
to the GitHub repository (https://github.com/rhiever/webstep-sklearn-quickstart-2019) in
your browser and click the green “Download” button in the upper right.

![](images/download-repo.png)

Please note that we may add and improve the material until shortly before the
tutorial session, and we recommend you to update your copy of the materials one
day before the tutorials. If you have an GitHub account and cloned the
repository via GitHub, you can sync your existing local repository with:

```bash
git pull origin master
```

If you don’t have a GitHub account, you may have to re-download the .zip
archive from GitHub.


Installation Notes
------------------

This tutorial will require recent installations of

- [NumPy](http://www.numpy.org)
- [SciPy](http://www.scipy.org)
- [matplotlib](http://matplotlib.org)
- [pandas](http://pandas.pydata.org)
- [pillow](https://python-pillow.org)
- [scikit-learn](http://scikit-learn.org/stable/)
- [TPOT](https://pypi.python.org/pypi/TPOT/)
- [IPython](http://ipython.readthedocs.org/en/stable/)
- [Jupyter Notebook](http://jupyter.org)


The Jupyter Notebook installation is important and you should be able to type:

    jupyter notebook

in your terminal window and see the notebook panel load in your web browser.
Try opening and running a notebook from the material to see check that it works. Alternatively you can use Jupyter Lab.

For users who do not yet have the required packages installed, a relatively
painless way to install all the requirements is to use a Python distribution
such as [Anaconda](https://www.anaconda.com/download/ "Anaconda"), which includes
the most relevant Python packages for science, math, engineering, and
data analysis; Anaconda can be downloaded and installed for free
including commercial use and redistribution.
The code examples in this tutorial should be compatible to Python 2.7,
Python 3.4-3.7.

After obtaining the tutorial material, we **strongly recommend** you to open and execute
the Jupyter Notebook `jupter notebook check_env.ipynb` that is located at the
top level of this repository. Inside the repository, you can open the notebook
by executing

```bash
jupyter notebook check_env.ipynb
```

inside this repository. Inside the Notebook, you can run the code cell by
clicking on the "Run Cells" button as illustrated in the figure below:

![](images/check_env-1.png)


Finally, if your environment satisfies the requirements for the tutorials, the
executed code cell will produce an output message as shown below:

![](images/check_env-2.png)

If any of the installations fail, you can install the packages using either `pip` or `conda`:

- `pip install [package-name]`  
- or `conda install [package-name]`

Although not required, we also recommend that you update the scikit-learn the latest release version to ensure best compatibility with the teaching material. Please upgrade already installed packages by executing:

- `pip install --no-deps --upgrade [package-name]`  
- or `conda update [package-name]`

Depending on how you installed ``scikit-learn``.


Data Downloads
--------------

The data for this tutorial is not included in the repository.  We will be
using several data sets during the tutorial: most are built-in to
scikit-learn, which
includes code that automatically downloads and caches these
data.

**Because wireless network connections can often be spotty, it would be a good idea to download these
data sets before arriving at the workshop.
Please run**
```bash
python fetch_data.py
```
**to download all necessary data beforehand.**

The download size of the data files are approx. 280 MB, and after `fetch_data.py`
extracted the data on your disk, the ./notebook/dataset folder will take 480 MB
of your local hard drive.


Outline
=======

Day 1 Session
---------------

- 01 Introduction to machine learning with sample applications, Supervised and Unsupervised learning [[view](notebooks/01.Introduction_to_Machine_Learning.ipynb)]
- 02 Scientific Computing Tools for Python: NumPy, SciPy, and matplotlib [[view](notebooks/02.Scientific_Computing_Tools_in_Python.ipynb)]
- 03 Data formats, preparation, and representation [[view](notebooks/03.Data_Representation_for_Machine_Learning.ipynb)]
- 04 Supervised learning: Training and test data [[view](notebooks/04.Training_and_Testing_Data.ipynb)]
- 05 Supervised learning: Estimators for classification [[view](notebooks/05.Supervised_Learning-Classification.ipynb)]
- 06 Supervised learning: Estimators for regression analysis [[view](notebooks/06.Supervised_Learning-Regression.ipynb)]
- 07 Unsupervised learning: Unsupervised Transformers [[view](notebooks/07.Unsupervised_Learning-Transformations_and_Dimensionality_Reduction.ipynb)]
- 08 Unsupervised learning: Clustering [[view](notebooks/08.Unsupervised_Learning-Clustering.ipynb)]
- 09 The scikit-learn estimator interface [[view](notebooks/09.Review_of_Scikit-learn_API.ipynb)]
- 10 Preparing a real-world dataset (titanic) [[view](notebooks/10.Case_Study-Titanic_Survival.ipynb)]
- 11 Working with text data via the bag-of-words model [[view](notebooks/11.Text_Feature_Extraction.ipynb)]
- 12 Application: SMS spam classification [[view](notebooks/12.Case_Study-SMS_Spam_Detection.ipynb)]

Day 2 Session
-----------------

- 13 Cross-Validation [[view](notebooks/13.Cross_Validation.ipynb)]
- 14 Model complexity and grid search for adjusting hyperparameters [[view](notebooks/14.Model_Complexity_and_GridSearchCV.ipynb)]
- 15 Scikit-learn Pipelines [[view](notebooks/15.Pipelining_Estimators.ipynb)]
- 16 Supervised learning: Performance metrics for classification [[view](notebooks/16.Performance_metrics_and_Model_Evaluation.ipynb)]
- 17 Supervised learning: Linear Models [[view](notebooks/17.In_Depth-Linear_Models.ipynb)]
- 18 Supervised learning: Decision trees and random forests, and ensemble methods [[view](notebooks/18.In_Depth-Trees_and_Forests.ipynb)]
- 19 Supervised learning: feature selection [[view](notebooks/19.Feature_Selection.ipynb)]
- 20 Unsupervised learning: Hierarchical and density-based clustering algorithms [[view](notebooks/20.Unsupervised_learning-Hierarchical_and_density-based_clustering_algorithms.ipynb)]
- 21 Unsupervised learning: Non-linear dimensionality reduction [[view](notebooks/21.Unsupervised_learning-Non-linear_dimensionality_reduction.ipynb)]
- 22 Unsupervised learning: Anomaly detection [[view](notebooks/22.Unsupervised_learning-anomaly_detection.ipynb)]
- 23 Automated machine learning [[view](notebooks/23.Automated_machine_learning.ipynb)]
