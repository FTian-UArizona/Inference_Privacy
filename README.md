# Inference Privacy: Properties and Mechanisms

This repository contains the code and data for the paper:

> **Inference Privacy: Properties and Mechanisms**  
> Fengwei Tian, Ravi Tandon  
> Asilomar Conference on Signals, Systems, and Computers, 2024 · [arXiv](https://arxiv.org/abs/2411.18746)

## Description

Ensuring privacy during inference stage is crucial to prevent malicious third parties from reconstructing users’ private inputs from outputs of public models. 
Despite a large body of literature on privacy preserving learning (which ensures privacy of training data), there is no existing systematic framework to ensure the privacy of users’ data during inference. 
Motivated by this problem, we introduce the notion of Inference Privacy (IP), which can allow a user to interact with a model (for instance, a classifier, or a chat-bot) while providing a rigorous privacy guarantee for the users’ data at inference. 
In this paper, we establish fundamental properties of the IP privacy notion and also contrast it with the notion of Local Differential Privacy (LDP). We next present two types of mechanisms for achieving IP: namely, input perturbations and output perturbations which are customizable by the users and can allow them to navigate the trade-off between utility and privacy. 
Through a series of experiments across various datasets, we demonstrate the usefulness of our framework and highlight the resulting trade-offs between utility and privacy during inference.

## Key Files and Folders
This repository contains two separate folders for each dataset: CIFAR10, and CIFAR100. 

*   Contains the scripts used for implementing the various mechanisms for each dataset. 
*   `LICENSE`: License information for the code and data.

## Running the Code

Each script is an independent notebook. Follow the instructions inside each notebook.

## Citation

```bibtex
@inproceedings{tian2024inference,
  title     = {Inference Privacy: Properties and Mechanisms},
  author    = {Tian, Fengwei and Tandon, Ravi},
  booktitle = {Asilomar Conference on Signals, Systems, and Computers},
  year      = {2024}
}
```
