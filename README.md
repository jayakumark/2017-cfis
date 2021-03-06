# CFIS WS ML: Lab Exercices

This repository contains several ipython notebooks with machine learning tutorials using python, keras and tensorflow.

## Contents

1. [Installation](#installation)
2. [Setup](#setup)
3. [Sessions](#sessions)
4. [Usage](#usage)


## Installation

- Install git (instructions [here](https://git-scm.com/downloads)).
- Clone this repository ```git clone https://github.com/telecombcn-dl/2017-cfis.git```

### Python

- Linux and MacOSX users: python 2.7 and 3.x are supported. Install from [official website](https://www.python.org/) or use [Anaconda](https://www.continuum.io/downloads)
- Windows users: only Anaconda with python 3.5 is supported (follow detailed steps below).

### Dependencies

Follow the instructions for your OS to install tensorflow. It is recommended that you install the CPU version of tensorflow, since the GPU version requires cuda and cudnn installed. If you are feeling adventurous and have a GPU, you can follow the instructions in the tensorflow website to do the installation of the GPU version.

#### Linux & Mac OS X

- Follow [these instructions](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/g3doc/get_started/os_setup.md#pip-installation) to install tensorflow with pip.
- Install other dependencies with ```pip install -r requirements.txt```

#### Windows

- Install [Anaconda3-4.2.0 X64](https://repo.continuum.io/archive/Anaconda3-4.2.0-Windows-x86_64.exe). It is important that you download this exact version of Anaconda. Otherwise tensorflow installation will likely fail.
- Download and install [Visual C++ 2015 Build Tools](http://landinghub.visualstudio.com/visual-cpp-build-tools).
- Run ```cmd.exe``` as admin.
- Run the following commands:

```shell
conda install conda=4.2.11
conda create -n tf python=3.5
activate tf
conda install jupyter
conda install h5py
conda install scipy
```

- Install Tensorflow:

```
# CPU only
pip install tensorflow
# GPU-enabled
pip install tensorflow-gpu
```

- Install other dependencies ```pip install -r requirements_win.txt```
- Note that at the beginning of every session, you must run ```activate tf``` before running the notebooks.


## Setup & Check installation

Run ``` python setup.py``` to collect datasets and models before we begin, to avoid problems if notebooks freeze at some point.
If you successfully run ```setup.py```, you are all set for the lab sessions ! If not, please let us know in the issues section and we will try to help you.

## Sessions

- [Deep Networks](sessions/mlp.ipynb)
- [Convolutional Neural Networks](sessions/convnets.ipynb)
- [Visualization](sessions/visualization.ipynb)
- [Deep Dream](sessions/dream.ipynb)


## Usage

All sessions will be run in IPython notebook. To start editing them run:

```shell
jupyter notebook
```

Then navigate to ```localhost:8888``` and start editing.
