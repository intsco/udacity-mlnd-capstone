# Udacity: Machine Learning Engineer Nanodegree
## Capstone Proposal and Capstone Project

This repository contains all the information needed to reproduce the
results of the Udacity MLND Capstone Project:
Classification of imaging mass spectrometry ion images provided by
european project [METASPACE](http://metaspace2020.eu).

### Input Data

Download and unpack the input data from AWS S3

```
wget https://s3-eu-west-1.amazonaws.com/intsco-datasets/udacity_mlnd_capstone_image_classes.tar.gz
tar -xvf udacity_mlnd_capstone_image_classes.tar.gz
```

All the needed data will be extracted into `image_classes` directory.

### Code and Software Dependencies

The code can be found in the `train_cnn.ipynb` Jupyter Notebook.
The notebook above has the following dependencies:
* Tensorflow>=1.4
* Keras>=2.06
* Pandas>=0.20
* Numpy>=1.13
* Matplotlib>=2

The code can be run on a CPU but using GPUs is highly recommeneded due to
long network training time.
We used a *p2.xlarge* AWS GPU instance with one *NVIDIA Tesla K80*.
For easy start, one of the public Ubuntu images with most dependencies
preinstalled can be used.

