# 50.040 Natural Language Processing Final Project

## nlp-scratch-gpt2

> [!NOTE]
>
> #### Setup Procedure
>
> 1. Download and unzip datasets [`XNLI-1.0.zip`](https://dl.fbaipublicfiles.com/XNLI/XNLI-1.0.zip) and [`XNLI-MT-1.0.zip`](https://dl.fbaipublicfiles.com/XNLI/XNLI-MT-1.0.zip) into root folder.
> 2. Create a new Python environment (or not, up to you) and set the environment for the `.ipynb` project file to the environment.
> 3. After creating your Python environment, run the following commands:
>
> ```zsh
> # Running locally
> source .venv/bin/activate
> pip install -r requirements.txt
>
> # On google-colab
> pip install -r requirements_colab.txt
> ```
>
> We recommended `python@3.11` for this project.  
> 4. Download fine-tuned model for downstream tasks from **Task 2** onwards by going to **HuggingFace** with this link: [model](https://huggingface.co/vancenceho/scratch-gpt-2/tree/main) **OR** enter the following command (_if you have hf command in your terminal_):
>
> ```zsh
> hf download vancenceho/scratch-gpt-2
>
> OR
>
> git clone https://huggingface.co/vancenceho/scratch-gpt-2
> ```
>
> 5. Place downloaded `scratch-gpt-2-model.pt` into `best_model` folder.
> 6. If you have done the steps correctly, your project directory should look like [this](#project-structure).

## Description

This is a team project. You are encouraged to form teams in any way you like, but each team must consist of either 4 or 5 people.

## Project Summary

In this project, our overall goal is building GPT-2 from scratch. We implement the GPT-2 architecture together with an optimizer, and then conduct a toy pretraining experiment. Next, we then set up a Natural Language Processing (_NLP_) task to a multilingual setting. Finally, we explore open-ended extensions and propose improvements based on our findings. Specifically, we are tasked to perform the following tasks:

- **Task 1: Implement GPT-2**
- **Task 2: English Natural Language Inference (_NLI_) with GPT-2**
- **Task 3: Multilingual NLI with GPT-2**
- **Extended Task 1: Extending GPT-2 to Machine Translation**
- **Extended Task 2: Attention Patterns & Layer Representations via Visualisations**
- **Extended Task 3: Replacing GPT-2 with Qwen (_Qwen2-0.5B_)**

Refer to [Project Documentation](./docs/default-final-project.pdf) for more detailed information on the specific tasks and feel free to check out our proposal for this project [here](./docs/50.040-nlp-project-proposal.pdf)!

Additionally, if you would like to have a more detailed view on our findings, feel free to take a look at our [experiments](./default_final_project.ipynb) and for a better view on the visualisations produced, you can always view them in the [outputs](./outputs/) directory.

> [!TIP]
>
> - Keep [Project Documentation](./docs/default-final-project.pdf) open while working
> - You can download this entire repository and save it to your Google Drive and mount it using the following command if you wish to work on this project on **Google Colab**
>
> ```zsh
> from google.colab import drive
> drive.mount('/content/drive')
> ```
>
> - Remember to switch your working directory after mounting!
> - Happy coding :)

## Project Structure

```zsh
best_model/
├── model.pt                                  # HuggingFace model
└── .gitkeep
config.py                                     # configurations for project
docs/
├── default-final-project.pdf                 # project documentation
├── 50.040-nlp-project-proposal.pdf           # project proposal
├── 50.040-nlp-final-project-report.pdf       # project report
└── *.pdf
utils.py                                      # helper functions
optimizer_test.npy                            # GPT-2 official weights
outputs/
└── *.png                                     # visualisations from code
default_final_project.ipynb                   # project notebook
pretrain.txt                                  # data for task1
XNLI-1.0/                                     # downloaded dataset
XNLI-MT-1.0/                                  # downloaded dataset
requirements.txt                              # local requirements
requirements-colab.txt                        # google-colab requirements
.gitignore
README.md                                     # Check this first!
LICENSE

```

## Acknowledgements

This dataset is from an awesome group of researchers from Facebook AI and New York University.

You can check out more about the dataset [here](https://github.com/facebookresearch/XNLI)!

This project is an undertaking of the [50.040 - Natural Language Processing](https://isakzhang.github.io/courses/50040-nlp.html#grading) module during Fall 2025 under the **_Information Systems Technology & Design_ (ISTD)** faculty at the **_Singapore University of Technology & Design_ (SUTD)**

All contents of this project are credited to:  
Copyright &copy; Prof. Zhang Wenxuan &nbsp;|&nbsp; ISTD &nbsp;|&nbsp; SUTD  
Copyright &copy; Vancence Ho &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;|&nbsp; CSD &nbsp;|&nbsp; SUTD  
Copyright &copy; Lee Ruiyu &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;|&nbsp; DAI &nbsp;|&nbsp; SUTD  
Copyright &copy; Justin Cho &nbsp; &nbsp;&nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;|&nbsp; CSD &nbsp;|&nbsp; SUTD

---
