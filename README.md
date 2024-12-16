# Hypergraph Random Walk Graph Neural Networks
This repository is the official implementation of [Hypergraph Random Walk Graph Neural Networks](https://drive.google.com/drive/folders/1v8zxelYlHdGsTbcId0X6pRHAIKWKBOhk?usp=sharing). 

This repo is a fork off the original [RWGNN Repository](https://github.com/giannisnik/rwgnn) and combines code from [vgae pytorch](https://github.com/DaehanKim/vgae_pytorch).


## Requirements

Code is written in Python 3.6 and all requirements are in `requirements.txt`

### Datasets
Use the following link to download datasets: 
```
https://ls11-www.cs.tu-dortmund.de/staff/morris/graphkerneldatasets
```
Extract the datasets into the `datasets` folder.

## Training and Evaluation

To train and evaluate the model in the paper run the notebook `main.ipynb`. Tunable hyperparameters and dataset configurations are listed at the top of the file. `args` controls the arguments for the RWGNN training portion and `vgae_args` controls the arguments for the VGAE inference portion. All parameters used are documented in our paper.

## Synthetic data

To create the synthetic dataset used in our paper, run the `gen_syn_data.ipynb` notebook and move the datasets generated and change the `main.ipynb` `args.dataset` to `"graph"`.