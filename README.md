<span style="color:red">Note: The code will be made publicly available once the paper is accepted.</font>
# PGCL: Prior-Guided Cooperative Learning for 2D Atmospheric Turbulence Strength Estimation and Infrared Image Restoration
This repository contains the implementation of the Prior-Guided Cooperative Learning (PGCL) framework as described in our paper "Joint 2D Atmospheric Turbulence Strength Estimation and Infrared Image Restoration Using Optics Prior Guided Cooperative Learning". PGCL introduces a novel approach for atmospheric turbulence measurement and infrared image restoration, integrating two transformer-based models - TMNet and TRNet - guided by optical priors.

## Features
- **TMNet**: Estimates turbulence strength (TS) providing optics knowledge for image restoration.
- **TRNet**: Restores infrared image sequences using TS prior.
- **$C_n^2$-Guided Frequency Loss**: Enables focused training in regions of strong turbulence.
- **1:1 Mixed Training**: Enhances the accuracy and generalizability in predicting 2D TS.

## Requirements
- Python 3.x
- PyTorch
- Additional dependencies are listed in `requirements.txt`.

## Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/naturezhanghn/PGCL.git
cd PGCL
pip install -r requirements.txt
```

## Usage
To train the model using the provided dataset:
```bash
python train.py --dataset_path "/path/to/dataset"
```

## Dataset
We used the Turbulence-distorted Infrared Imaging Dataset (TIID) for training and evaluation. For more details, refer to the dataset [here](https://zenodo.org/records/8002688).

