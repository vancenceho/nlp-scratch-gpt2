# kp-gpt2-nlp

50.040 Natural Language Processing Project - Fall 2025

> [!NOTE]
>
> #### Setup Procedure
>
> 1. Download and unzip datasets `pretrain.txt`, `XNLI-1.0.zip` and `XNLI-MT-1.0.zip` into root folder.
> 2. Create a new Python environment (or not, up to you) and set the environment for the `.ipynb` project file to the environment.
> 3. After creating your Python environment use `pip` to install `requirements.txt`
>    > > recommended `python@3.11` for this project.
> 4. Download fine-tuned model for downstream tasks from **Task 2** onwards by going to **HuggingFace** with this link: [model](https://huggingface.co/vancenceho/scratch-gpt-2/tree/main) **OR** entering the following command (_if you have hf command in your terminal_):
>
> ```zsh
> hf download vancenceho/scratch-gpt-2
>
> OR
>
> git clone https://huggingface.co/vancenceho/scratch-gpt-2
> ```

## Description

This is a team project. You are encouraged to form teams in any way you like, but each team must consist of either 4 or 5 people.

## Project Summary

In this project, our overall goal is building GPT-2 from scratch. We implement the GPT-2 architecture together with an optimizer, and then conduct a toy pretraining experiment. Next, we then set up a Natural Language Processing (_NLP_) task to a multilingual setting. Finally, we explore open-ended extensions and propose improvements based on our findings. Specifically, we are tasked to perform the following tasks:

- **Task 1: Implement GPT-2**
- **Task 2: English Natural Language Inference (_NLI_) with GPT-2**
- **Task 3: Multilingual NLI with GPT-2**
- **Task 4: Extended Tasks with Improvements**

## Acknowledgements

This dataset is from an awesome group of researchers from Facebook AI and New York University.

You can check out more about the dataset [here](https://github.com/facebookresearch/XNLI)!

This project is an undertaking of the [50.040 - Natural Language Processing](https://isakzhang.github.io/courses/50040-nlp.html#grading) module during Fall 2025 under the _**Information Systems Technology & Design**_ faculty at the _**Singapore Unverisyt of Technology & Design**_

All contents of this project are credited to:  
Copyright &copy; Prof. Zhang Wenxuan &nbsp;|&nbsp; ISTD &nbsp;|&nbsp; SUTD  
Copyright &copy; Vancence Ho &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;|&nbsp; CSD &nbsp;|&nbsp; SUTD  
Copyright &copy; Lee Ruiyu &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;|&nbsp; DAI &nbsp;|&nbsp; SUTD  
Copyright &copy; Justin Cho &nbsp; &nbsp;&nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;|&nbsp; DAI &nbsp;|&nbsp; SUTD

---
