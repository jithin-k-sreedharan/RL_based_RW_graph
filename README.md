# Reinforcemnt Learning based Random Walks on Graphs

This repository provides implementation of certain random walk based graph exploration and estimation techniques given in the following paper
* [Revisiting Random Walk based Sampling in Networks: Evasion of Burn-in Period and Frequent Regenerations](https://computationalsocialnetworks.springeropen.com/track/pdf/10.1186/s40649-018-0051-0?site=computationalsocialnetworks.springeropen.com) \
(alphabetical order) Konstantin Avrachenkov, Vivek S. Borkar, Arun Kadavankandy and Jithin K. Sreedharan\
_Computational Social Networks, Springer, 2018_

The main algorithm is the reinforcement learning based random walk crawling algorithm that does not us to drop the initial burn-in samples.  

The data is taken from SNAP repository and Newman's repository.

## Prerequisites
Python 3+ installation with the following additional packages:
* Networkx
* NumPy
* Matplotlib
* Pickle
* Pandas

## Running
The Jupyter Notebook `model_run.ipynb` and the dataset files `friendster_community1_trimmed.edgelist` and `lesmis.edgelist` contain everything needed to run the experiments in the papers. The Notebook file also contains implementations of popular random walk techniques for comparing with our technique.

## Data
We have collected data from Friendster online social network and the edgelist of one of the largest connected component is shared with this repo. We have also shared the edgelist of the Les Miserables network.
