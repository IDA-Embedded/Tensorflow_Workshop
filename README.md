# Tensorflow Workshop.
This repository contains the code for the Tensorflow Workshop used in IDA Embedded for EoT 2023.

## Table of Contents.
- [References.](#references)
- [Requirements.](#requirements)
- [Introduction.](#introduction)
- [Workshop.](#workshop)
  - [1. Installation of Tensorflow and its dependencies.](#1-installation-of-tensorflow-and-its-dependencies)
    - [Creating an virtual environment (Python 3.8).](#creating-an-virtual-environment-python-38)
    - [Installing Tensorflow.](#installing-tensorflow)
    - [Installing different dependencies.](#installing-different-dependencies)
  - [2. Capturing images and annotating them using LabelImg.](#2-capturing-images-and-annotating-them-using-labelimg)
    - [Capturing images.](#capturing-images)
    - [Annotating images.](#annotating-images)
  - [3. Training a model using Tensorflow and exporting to Tensorflow Light.](#3-training-a-model-using-tensorflow-and-exporting-to-tensorflow-light)
    - [Training a model.](#training-a-model)
    - [Exporting the model to Tensorflow Light.](#exporting-the-model-to-tensorflow-light)
  - [4. Testing the model using Tensorflow.](#4-testing-the-model-using-tensorflow)
    - [Testing the model.](#testing-the-model)


## References.
This notebook is inspired by [Tensorflow Object Detection Walkthrough](https://github.com/nicknochnack/TFODCourse) offered by nicknochnack.

## Requirements.
This workshop is requiring the following:
- Ubuntu 20.04 ( or any other Linux distribution, but we have only tested it on Ubuntu 20.04 )
- Python 3.8
- VSCode ( Link : https://code.visualstudio.com/download )


## Introduction.
Tensorflow is an open-source software library for machine learning. It is used for both research and production. It was developed by Google Brain Team for internal Google use. It is an end-to-end open source platform for machine learning. It has a comprehensive, flexible ecosystem of tools, libraries, and community resources that lets researchers push the state-of-the-art in ML and developers easily build and deploy ML powered applications. In this workshop, we are going to use Tensorflow to train a model that can detect objects. We are going to use the model to detect objects in images captured using our built-in camera. The aim of this workshop is to showcase how easy it is to use Tensorflow to train a model and use it to detect objects in images. We will be exporting our trained model to tensorflow light so that it is ready for deployment on an embedded linux target such as a Raspberry Pi. We are going to use the following tools:
- Tensorflow: Used to train a model.
- LabelImg: Used to annotate images.
- OpenCV: Used to capture images.
- Numpy: Used to manipulate images.
- Matplotlib: Used to display images.


## Workshop.
The workshop is acting as a cookbook for the Tensorflow framework. It is divided into 4 parts:
1. Installation of Tensorflow and its dependencies.
2. Capturing images and annotating them using LabelImg.
3. Training a model using Tensorflow and exporting to Tensorflow Light.
4. Testing the model using Tensorflow.
## 1. Installation of Tensorflow and its dependencies.
### Creating an virtual environment (Python 3.8).
We are going to use a virtual environment to install Tensorflow and its dependencies. This is done to avoid conflicts with other Python packages.
### Installing Tensorflow.
We are going to install Tensorflow using the pip package manager. We are going to install the CPU version of Tensorflow to simplify installation.
Please note that installing tensorflow for GPU is a bit more complicated but it is recommended for better performance.
### Installing different dependencies.
We are going to install the following dependencies:
- LabelImg: Used to annotate images.
- OpenCV: Used to capture images.
- Numpy: Used to manipulate images.
- Matplotlib: Used to display images.
- protobuf: Used to export the model to Tensorflow Lite.
## 2. Capturing images and annotating them using LabelImg.
We are using our built-in camera to capture images. We are going to capture 10 images of the same object. We are going to use LabelImg to annotate the images.
### Capturing images.
We are going to capture 10 images of the same object. We are going to use OpenCV to capture the images.
### Annotating images.
We are going to use LabelImg to annotate the images. LabelImg is a graphical image annotation tool and label object bounding boxes in images. It is written in Python and uses Qt for its graphical interface.
## 3. Training a model using Tensorflow and exporting to Tensorflow Light.
We are going to use Tensorflow to train a model. We are going to use the images captured in the previous step to train the model. We are going to use Tensorflow Light to export the model.
### Training a model.
This part of the workshop is a Shift-Enter exercise, we are not going to provide much information about it. The goal is to train a model using Tensorflow. The model should be able to detect the object we captured the images of.
### Exporting the model to Tensorflow Light.
We are going to use Tensorflow Light to export the model. Tensorflow Light is a set of tools to help developers run TensorFlow models on mobile, embedded, and IoT devices. It enables on-device machine learning inference with low latency and a small binary size.
## 4. Testing the model using Tensorflow.
We are going to use Tensorflow to test the model. 
### Testing the model.
We will again use the built-in camera to capture images. We are going to use the model we trained in the previous step to detect the object in the images. We are going to use OpenCV to display the images.