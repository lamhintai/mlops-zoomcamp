# 1. Introduction

## 1.2 Environment preparation

I use GitHub Codespaces to run do this module.
Steps run so far:

### Step 1: Install miniforge

From my past working experience, I prefer to use mamba instead of conda for performance reason.

```sh
wget "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh
```

Accept auto-activating the base environment and then restart the terminal. In case we need to manually set the auto-activating the base environment, run:

```sh
conda config --set auto_activate_base true
```

### Step 2: Create environment and install Python packages

We will need to install Jupyter notebook, pandas, seaborn, scikit-learn and pyarrow to run the assignment later.

```sh
mamba create -n zoomcamp
conda activate zoomcamp

mamba install notebook pandas scikit-learn seaborn pyarrow
```

Test if everything works:

```sh
juypter notebook
```
