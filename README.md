# DenseDepth Implemention in Pytorch
This repo contains Pytorch implementation of depth estimation deep learning network based on the published paper: [High Quality Monocular Depth Estimation via Transfer Learning](https://arxiv.org/pdf/1812.11941.pdf)

## Installation

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Requirements

This code was tested with:
* Ubuntu 18.04 with python 3.6.9

*The code also runs on Jetson TX2, for which all dependencies need to be installed via NVIDIA JetPack SDK.*


### Step-by-Step Procedure
In order to set the virtual environment, apriori installation of Anaconda3 platform is required.

Use the following commands to create a new working virtual environment with all the required dependencies.

**GPU based enviroment**:
```
git clone https://github.com/tau-adl/DenseDepth
cd DenseDepth_Pytorch
conda env create -f DenseDepth_env.yml
conda activate DenseDepth
pip install -r pip_requirements.txt
```

*In order to utilize the GPU implementation make sure your hardware and operation system are compatible for Pytorch with python 3*

### Data Collection

Run the shell script ```DataCollect.sh```

## Training the model

Execute training by running:  
```
python3 Train.py
```

## Testing the model

Execute testing by running:  
```
python3 Evaluate.py
```

## Authors

* **David Sriker** - *David.Sriker@gmail.com*
