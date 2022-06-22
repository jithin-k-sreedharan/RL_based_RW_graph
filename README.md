# Reinforcemnt Learning based Random Walks on Graphs

This repository provides the implementation of random walk based graph exploration and estimation techniques proposed in the paper (and some commonly used sampling algorithms):
> [Revisiting Random Walk based Sampling in Networks: Evasion of Burn-in Period and Frequent Regenerations](https://computationalsocialnetworks.springeropen.com/track/pdf/10.1186/s40649-018-0051-0?site=computationalsocialnetworks.springeropen.com) \
(_alphabetical order_) Konstantin Avrachenkov, Vivek S. Borkar, Arun Kadavankandy, and Jithin K. Sreedharan\
_Computational Social Networks, Springer, 2018_

The main algorithm is the **reinforcement learning based random walk crawling algorithm** that does not require us to drop the initial burn-in samples. The repo contains implementations of the following random walk on graph algorithm:
* Metropolis–Hastings sampling
* Respondent-driven sampling
* Reinforcement learning based algorithm with Metroplis-Hasting sampling as the backbone 
* Reinforcement learning based algorithm with lazy random walk as the backbone
* Reinforcement learning based algorithm with with stanard (simple) random walk as the backbone
* Ratio with tours estimator 

## Prerequisites
Python 3+ installation with the following additional packages:
* Networkx
* NumPy
* Matplotlib
* Pickle
* Pandas

## Running
The Jupyter Notebook `model_run.ipynb` and the dataset files `friendster_community1_trimmed.edgelist` and `lesmis.edgelist` contain everything needed to run the experiments in the papers. The Notebook file also includes implementations of popular random walk techniques for comparing with our approach.

## Data
We have used data from Friendster online social network (one of the largest connected components) and a network formed from Les Misérables novel. This repository includes the edge list of both networks.
