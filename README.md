# Surface Energy Manuscript

This repository contains various scripts/notebooks we used to create the results in our paper.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Usage](#usage)
  - [Cleavage energy dataset](#surface-energy-dataset)
  - [Train a CGCNN model](#train-a-cgcnn-model)


## Prerequisites
* Crystal Graph Convolutional Neural Networks ([CGCNN](https://github.com/ulissigroup/cgcnn/tree/sklearn_refactor))

* Additional packages required for cgcnn environmnet:
- [PyTorch](http://pytorch.org)
- [scikit-learn](http://scikit-learn.org/stable/)
- [pymatgen](http://pymatgen.org)
- AdamW

## Usage

### Cleavage energy dataset

Located in the `cleavage_energy_dataset` folder. 

We have included a pickel file that contain our cleavage energy data, along with a Jupyter notebook (`read_data.ipynb`).

### Train a CGCNN model

Located in the `train_CGCNN_model` folder.

We have included the cgcnn we used, and `random_asgginment` method. `random_assignment.ipynb` notebook splits the data randomly into 8:2 training: test set, and uses CGCNN to train a model. **You need to clone the CGCNN repository and install all the prerequisite packages in order to run these notebooks** 

We have included the optimized paramters we used for CGCNN: 
"atom_fea_len": 43, <br/>
"batch_size": 87, <br/>
"step": "0.1", <br/>
"epochs": 218, <br/>
"h_fea_len": 114, <br/>
"log_learning_rate": -6.465085550816676, <br/>
"n_conv": 8, <br/>
"n_h": 3, <br/>
"max_num_nbr": 12, <br/>
"optimizer": "AdamW"

