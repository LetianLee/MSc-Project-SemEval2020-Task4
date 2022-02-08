*The project code was completed on September 10, 2021.*

# MSc Project: Commonsense Validation and Explanation in Natural Language Processing

[<img src="https://raw.githubusercontent.com/pytorch/pytorch/master/docs/source/_static/img/pytorch-logo-dark.png" width="10%">](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)   

This is the source code for the MSc Project: **Commonsense Validation and Explanation in Natural Language Processing**. The project is aiming to solve the first two subtasks in [*SemEval 2020 Task 4 - Commonsense Validation and Explanation (ComVE)*](https://competitions.codalab.org/competitions/21080).  



## Project Information
* **Title:** Commonsense Validation and Explanation in Natural Language Processing<br>
* **Objective Task:** SemEval 2020 Task 4 - Commonsense Validation and Explanation (ComVE)<br>
* **Supervisor:** Dr Mark Lee<br>
* **Student:** Letian Li (2214560)



## Task Description
This MSc project contains two subtasks.  

**Subtask A** is a Validation task. The purpose is to determine which of two similar natural language statements is against common sense.

*Example:*  
> **Task:** Which of the two statements is against common sense?  
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
First, to implement this work, you need to download and install Anaconda3. Here is the official link for Anaconda: https://www.anaconda.com/products/individual-d  
After installing the appropriate version of Anaconda3, please execute the following command block on the console. (The example below is based on the Linux operating system.)

```bash
# Create a conda envs
conda create -n msc_project_2214560 python=3.7 ipython
conda activate msc_project_2214560

# Install PyTorch 
# Please Note: Install the appropriate version of PyTorch, and be aware of your operating system and CUDA version. Please check https://pytorch.org/get-started/locally/ 
# The following command is for the PyTorch installation of Linux operating system and CUDA 10.2.
pip install torch torchvision torchaudio

# Install HuggingFace Transformers
pip install transformers==4.9.1

# Install other libraries
pip install TensorBoard==2.6.0
pip install jupyter==1.0.0
pip install pandas==1.2.4
pip install matplotlib==3.3.4
pip install seaborn==0.11.1
```

### 2. Viewing and Running the Project Code
After installing the project environment, you can run Jupyter Notebook to view and run the project.

### 3. The Directory Tree of Project
```
MSc Project (Commonsense Validation and Explanation in Natural Language Processing)
├── MSc Project
│   ├── Best Implementation
│   │   ├── Subtask_A.ipynb -------------------------- This is the best implementation for subtask A.
│   │   └── Subtask_B.ipynb -------------------------- This is the best implementation for subtask B.
│   ├── DataSet -------------------------------------- This is the DataSet of the SemEval-2020 Task 4.
│   └── Experiment
│       ├── ExperimentResult_A ----------------------- This keeps the experiment results of subtask A. (New results will be generated automatically)
│       ├── ExperimentResult_B ----------------------- This keeps the experiment results of subtask B. (New results will be generated automatically)
│       ├── TensorBoard ------------------------------ This keeps the TensorBoard records. (This directory will be generated automatically)
│       ├── Experiment Workflow.ipynb ---------------- This shows the experiment workflow and generates the result figures.
│       ├── Experiment_Subtask_A.ipynb --------------- This is the experiment code for subtask A.
│       └── Experiment_Subtask_B.ipynb --------------- This is the experiment code for subtask B.
├── Project Demonstration (updated).pdf -------------- This is the project demonstration slide.
└── README.md
```



## Suggestion
If you just want a quick look at how to solve the task, please see the implementation code:  
> [**MSc-Project-SemEval2020-Task4/MSc Project/Best Implementation/Subtask_A.ipynb**](https://github.com/LetianLee/MSc-Project-SemEval2020-Task4/blob/master/MSc%20Project/Best%20Implementation/Subtask_A.ipynb)  
> [**MSc-Project-SemEval2020-Task4/MSc Project/Best Implementation/Subtask_B.ipynb**](https://github.com/LetianLee/MSc-Project-SemEval2020-Task4/blob/master/MSc%20Project/Best%20Implementation/Subtask_B.ipynb)

If you want to know how the project conducts experiments, please see the experiment code:  
> [**MSc-Project-SemEval2020-Task4/MSc Project/Experiment/Experiment_Subtask_A.ipynb**](https://github.com/LetianLee/MSc-Project-SemEval2020-Task4/blob/master/MSc%20Project/Experiment/Experiment_Subtask_A.ipynb)  
> [**MSc-Project-SemEval2020-Task4/MSc Project/Experiment/Experiment_Subtask_B.ipynb**](https://github.com/LetianLee/MSc-Project-SemEval2020-Task4/blob/master/MSc%20Project/Experiment/Experiment_Subtask_B.ipynb)

If you want to take an overview of this project, please see the project demonstration slide:  
> [**MSc-Project-SemEval2020-Task4/Project Demonstration (updated).pdf**](https://github.com/LetianLee/MSc-Project-SemEval2020-Task4/blob/master/Project%20Demonstration%20(updated).pdf)  
