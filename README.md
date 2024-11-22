# [Inference Privacy]

This repository contains the code and data associated with the paper Inference Privacy: Properties and Mechanisms.

## Description

Ensuring privacy during inference stage is crucial to prevent malicious third parties from reconstructing users’ private inputs from outputs of public models. Despite a large body of literature on privacy preserving learning (which ensures privacy of training data), there is no existing systematic framework to ensure the privacy of users’ data during inference. Motivated by this problem, we introduce the notion of Inference Privacy (IP), which can allow a user to interact with a model (for instance, a classifier, or a chat-bot) while providing a rigorous privacy guarantee for the users’ data at inference. In this paper, we
establish fundamental properties of the IP privacy notion and also contrast it with the notion of Local Differential Privacy (LDP). We next present two types of mechanisms for achieving IP: namely, input perturbations and output perturbations which are customizable by the users and can allow them to navigate the trade-off between utility and privacy. Through a series of experiments across various datasets, we demonstrate the usefulness of our framework and highlight the resulting trade-offs between utility and privacy during inference.

## Key Files and Folders

*   `code/`: Contains the scripts used for implentating of verious mechanisms in CIFAR10 and CIFAR100 datasets.
*   `environment.yml`: [Description, e.g., Conda environment file with the required packages.]
*   `LICENSE`: License information for the code and data.

## Installation

[Provide clear instructions on how to set up the necessary environment and install the required dependencies.  This might include:]

1.  Clone the repository: `git clone https://github.com/your-username/your-repository.git`
2.  Create a conda environment (optional but recommended): `conda env create -f environment.yml`
3.  Activate the environment: `conda activate your_environment_name`
4.  Install additional packages (if any): `pip install -r requirements.txt`

## Running the Code

Each code is an indepedent Notebook File, please follow the instruction in each Notebook file. 
