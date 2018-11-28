# MOOC-Learner-Modeled

Serves as an interface to train and test all kinds of classifier models on all 
possible set of user longitudinal features, and transfer models among weeks and courses. It is consist of four parts:
- Data pool: gives an interface to fetch user longitudinal features along with dropouts and split feature dataframes 
into two parts for training and testing.
- Classifier pool: gives an interface to query, dump and load classifier models, and transfer 
them among weeks and courses.
- Training part: train a set models. Accept input a list of model configurations and a list of dataframes they trained 
on. It will then train a set of models for each unique combination of all configurations.
- Testing part: test multiple models on multiple dataframes for each unique combination of them. Publish and analyze 
the test results by means like ROC curves and accuracy and AUC tables.

# Requirements 

<a href="https://www.python.org/" ><img src="https://img.shields.io/badge/Python-blue.svg"></a>

<a href="https://www.docker.com/" ><img src="https://img.shields.io/badge/Docker-blue.svg"></a> 
(see [MOOC-Learner-Docker/modeled_base_img](https://github.com/MOOC-Learner-Project/MOOC-Learner-Docker/tree/master/modeled_base_img) )

## Technologies

<a href="https://www.pandas.pydata.org/" ><img src="https://img.shields.io/badge/Pandas-blue.svg"></a>
<a href="https://www.matplotlib.org/" ><img src="https://img.shields.io/badge/Matplotlib-blue.svg"></a>
<a href="https://www.numpy.org/" ><img src="https://img.shields.io/badge/Numpy-blue.svg"></a>
<a href="https://scikit-learn.org/stable/index.html" ><img src="https://img.shields.io/badge/Scikitlearn-blue.svg"></a>
<a href="http://flask.pocoo.org/" ><img src="https://img.shields.io/badge/Flask-blue.svg"></a>
<a href="http://redis.io" ><img src="https://img.shields.io/badge/redis-blue.svg"></a>


# Installation

See [MOOC-Learner-Docker](https://github.com/MOOC-Learner-Project/MOOC-Learner-Docker/tree/master/README.md)

# Tutorial

Entry point is `autorun.py`. Configuration is done with `config/*yml`, see e.g. `config/sample_config.yml`.

