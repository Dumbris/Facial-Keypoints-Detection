This is the working directory for the team Deep Learning Freelancers for the kaggle contest Facial Keypoints Detection
https://www.kaggle.com/c/facial-keypoints-detection

## Installation

### Ubuntu 14.04, 15.10

The simple way to install last version of Theano and lasagne using anaconda installer

- Go to https://docs.continuum.io/anaconda/install#id7 , do installation steps from Linux install section

- Install required packages with command
```
conda install -c https://conda.anaconda.org/Toli lasagne Theano nolearn tabulate
```

- execute carl/run.sh from repository

## Troubleshooting

In case of error 
ImportError: No module named cPickle

Change a line in kfkd_v1.py file
```
import cPickle as pickle
```
to
```
from six.moves import cPickle as pickle
```
