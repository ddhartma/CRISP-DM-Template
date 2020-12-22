# CRISP-DM reusable template

This repository can be used as a Template for CRISP- DM analysis (CROSS INDUSTRY STANDARD PROCESS FOR DATA MINING).

Each CRISP- DM should cover the important sections
- Business Understanding
- DataFrame Understanding
- DataFrame Preparation
- Modeling
- Evaluation

Further links to CRISP-DM can be found here:
- [CRISP-DM Overview- Data Science Project Management](https://www.datascience-pm.com/crisp-dm-2/)
- [Manage your next Data Science Project with CRISP-DM METHOD](https://analyticsindiamag.com/crisp-dm-data-science-project/)
- [Six steps in CRISP-DM the standard data mining process](https://www.proglobalbusinesssolutions.com/six-steps-in-crisp-dm-the-standard-data-mining-process/)

The following sections in this README can be used itself as a README template for specific CRISP-DM analysis.

## Business Understanding (aim of this study)
The aim of this study was to analyze via CRISP-DM (CROSS INDUSTRY STANDARD PROCESS FOR DATA MINING) if one can build model which can predict a special target based on the given dataset features.

The ***Business Understanding*** part covers the main question ***What does the business need?***. This question should be divided in separate  - more accurate - questions:

1. **Question 1:** ...?
2. **Question 2:** ...?
3. **Question 3:** ...?

## DataFrame Overview
- What is the shape of the dataset, how many numerical , how many categorical columns are there?
- **numerical** columns:
    - col1
    - col2
    - col3

- **categorical** columns:
    - col4
    - col5
    - col6

## Data understanding and preparation
The notebook **PLEASE_SPECIFY.ipynb** contains the dataset investigation steps and and all the results.

- **NaN values:** Describe the distribution of NaN values and the way they are handled (removed/imputed/calculated/modeled/ etc.)

- **0/special values:** Describe the distribution of 0 / specialö values and the way they are handled (removed/imputed/calculated/modeled/ etc.)

- **Dropping Columns:** Are there columns which can be dropped as they are not needed for modeling?

- **Creating Dummies:** Are there categorical variables for which dummy or binary variables are needed to build a predicting model


## Modeling:
- The main modeling approach in this Jupyter notebook is done based on a sklearn Linear Regression. The R-squared value (a measure of how much of the data variability can be explained by the model) is ABOUT ... for training and ... for testing.
- Are there nonlinear tendencies for some features-target-dependencies? Are there linearization steps included?
- Are there deep learning nonlinear model applied for predictions (Tensorflow, Pytorch)?

## Evaluation:
The answers to this CRISP questions and further information can be found in the jupyter notebook. The most important results are:
- **Answer to Question 1:** ...
- **Answer to Question 2:** ...
- **Answer to Question 3:** ...


## Read my blog post under medium

IN CASE THERE IS A BLOG POST FOR STAKEHOLDERS: Check out my [medium](https://hartmann-david.medium.com/how-do-you-become-a-famous-song-writer-ff3a4668a8c8) blog post.

## Setup Instructions

The following is a brief set of instructions on setting up a managed notebook instance, from which the notebooks can be completed and run.

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites: Installation of Python via Anaconda and Command Line Interaface
- Install [Anaconda](https://www.anaconda.com/distribution/). Install Python 3.7 - 64 Bit
- If you need a good Command Line Interface (CLI) under Windowsa you could use [git](https://git-scm.com/). Under Mac OS use the pre-installed Terminal.

- Upgrade Anaconda via
```
$ conda upgrade conda
$ conda upgrade --all
```

- Optional: In case of trouble add Anaconda to your system path. Write in your CLI
```
$ export PATH="/path/to/anaconda/bin:$PATH"
```

### Clone the project
- Open your Command Line Interface
- Change Directory to your project older, e.g. `cd my_github_projects`
- Clone the Github Project inside this folder with Git Bash (Terminal) via:
```
$ git clone https://github.com/ddhartma/CRISP-DM-Template.git
```

- Change Directory
```
$ cd crisp_dm_analysis
```

- Create a new Python environment. Inside Git Bash (Terminal) write:
```
$ conda create --name crisp_dm_analysis
```

- Install the following packages (via pip or conda)
```
numpy = 1.17.4
pandas = 0.24.2
matplotlib = 3.1.0
tensorflow = 1.14.0
seaborn = 0.9.0
scikit-learn = 0.21.2
```

- Check the environment installation via
```
$ conda env list
```

- Activate the installed crisp_dm_analysis environment via
```
$ conda activate crisp_dm_analysis
```

### Open and run the notebook
Now that the repository has been cloned into the notebook instance you may navigate to the notebook. Run the notebook via

```
jupyter notebook 0_CRISP_DM_template.ipynb
```
### Attached files in the repository
- **0_CRISP_DM_template.ipynb** - the main file of this repository containing a CRISP-DM analysis, all coding steps and the important results.
- **plot_df** - a helper module containing three functions:
  - plot_df_line
  - plot_df_bar
  - plot_df_pie

  This module simplifies plotting line, bar and pie plots using matplotlib. It is called from the notebook and shortens the code for specially designed plots to a 'one code line'. This is done via default settings and overwriting them only when needed.  

- **README.md** - the readme file of this repository.

## Acknowledgments
* The categorical CategoricalTransformer class in this work was developed by [Guy Kahana & Anat Peled](https://www.kaggle.com/anatpeled/spotify-popularity-prediction/comments)
