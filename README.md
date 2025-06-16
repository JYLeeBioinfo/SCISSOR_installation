Installation instruction for R package [SCISSOR](https://github.com/hyochoi/SCISSOR).


# 0 Install conda if there is none.
 - I recommend the installation of [miniforge version](https://github.com/conda-forge/miniforge).
 - Refer to the "install" section in the miniforge repo.

# 1 create environment
```
mamba env create -f environment.yml
```

 - If you want to install Rstudio also, run this instead.
```
mamba env create -f environment_with_rstudio.yml
```

 - If you want to use R from vscode, run this instead.
```
mamba env create -f environment_for_vscode.yml
```

# 2 Install remaining dependencies and SCISSOR
 - Activate SCISSOR environment and launch R console
```
mamba activate SCISSOR
R
```
 - And then install remaining dependencies and SCISSOR as follows.
```
devtools::install_github("cran/refGenome")
devtools::install_github("hyochoi/SCISSOR")
```
