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

There is one folder per dataset: `CIFAR10/` and `CIFAR100/`. Each folder contains:

*   `*_FineTune.ipynb`: grid search for fine-tuning the pretrained ResNet-18 under noise.
*   `*_test.ipynb`: Gaussian input, output, and mixed perturbation experiments; makes the figures.
*   `SLL.ipynb`: checks the Lipschitz constant of the SLL model.
*   `SLL/`: SDP-based Lipschitz Layer (SLL) code from the original authors (see Third-party code below).

The SLL model checkpoints (for example `SLL/modelsmall.ckpt`) are not included in this repository.

## Running the Code

Each script is an independent notebook. Follow the instructions inside each notebook.

## Third-party code

The `CIFAR10/SLL/` and `CIFAR100/SLL/` folders contain code from
[Lipschitz-SLL-Networks](https://github.com/araujoalexandre/Lipschitz-SLL-Networks)
by Alexandre Araujo, Aaron Havens, Blaise Delattre, Alexandre Allauzen, and Bin Hu
("A Unified Algebraic Perspective on Lipschitz Neural Networks", ICLR 2023).
That code is licensed under the Apache License 2.0. A copy of the license is in each `SLL/` folder.
We changed `models/model.py`, `data/readers.py`, and `utils.py` for this project. The other SLL files are unchanged.

## Citation

```bibtex
@inproceedings{tian2024inference,
  title     = {Inference Privacy: Properties and Mechanisms},
  author    = {Tian, Fengwei and Tandon, Ravi},
  booktitle = {Asilomar Conference on Signals, Systems, and Computers},
  year      = {2024}
}
```
