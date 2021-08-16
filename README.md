*Updated on August 16, 2021.*

# MSc Project (SemEval-2020 Task 4)

[<img src="https://raw.githubusercontent.com/pytorch/pytorch/master/docs/source/_static/img/pytorch-logo-dark.png" width="10%">](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)   

This is the source code for the MSc Project.  



## Project Information
* Title: Commonsense Validation and Explanation in Natural Language Processing<br>
* Objective Task: SemEval 2020 Task 4 - Commonsense Validation and Explanation (ComVE)<br>
* Supervisor: Dr Mark Lee<br>
* Student: Letian Li (2214560)



## Task Description
This MSc project contains two subtasks.  

**Subtask A** is a Validation task. The purpose is to determine which of two similar natural language statements is against common sense.

*Example:*  
> Task: Which of the two statements is against common sense?  
> Statement1: He put a turkey into the fridge.  
> Statement2: He put an elephant into the fridge. 

**Subtask B** is an Explanation (Multi-Choice) task. The purpose is to find the right reason why a given statement is against common sense.

*Example:*  
> **Task:** Select the most appropriate reason as to why this statement is against common sense.  
> **Statement:** He put an elephant into the fridge.  
> A: An elephant is much bigger than a fridge.  
> B: Elephants are usually white while fridges are usually white.  
> C: An elephant cannot eat a fridge.



## Instructions
Python 3.7 with PyTorch 1.9.0 and Transformers 4.9.1 serve as the backbones of this project.

The code is using one GPU by default, you have to modify the code to make it running on CPU or multiple GPUs.

### 1. Envs and Dependencies
```bash
# Create a conda envs
conda create -n msc_project_2214560 python=3.7 ipython
conda activate msc_project_2214560

# Install PyTorch 
# Note: If your compute platform is not CUDA 11.1, please check https://pytorch.org/get-started/locally/ for PyTorch INSTALLATION.
pip install torch==1.9.0+cu111 torchvision==0.10.0+cu111 torchaudio==0.9.0 -f https://download.pytorch.org/whl/torch_stable.html

# Install HuggingFace Transformers
pip install transformers==4.9.1
```
