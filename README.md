# alab_repo_template

## Intro

If you are a [A lab](https://albertsenlab.org/) member, you will probably create your own (sub)project repo or work on one that already exists.
Therefore, to ensure the interoperability among lab members and reproducibility among different labs, it is important to follow a common and documented operational standard.
This repo serves as:
1. A template for the repos of the A lab (sub)projects: you can copy one of the repo's branches depending on what your needs are;
2. A guide to how to setup a (sub)project repo: you can follow the workflow to create your own (sub)project.

## Repo structure

The repo is structured in a way that the folders and the subfolders store the contet in the least ambiguous way possible.

| Folder | Content |
| --- | --- |
| project_repo | The main repo of the (sub)project, in this case the [alab_repo_template](https://github.com/fdelogu/alab_repo_template). |
| ├── data/ | The input for the project. |
| │   ├── links/ | The [symbolic links](https://manpages.ubuntu.com/manpages/bionic/man8/sln.8.html) pointing to the raw (or consolidated) A lab data, which are stored separately. This ensures that the original data are protected form users' errors and avoids unnecessary data duplication. |
| │   ├── downloads/ | The raw data downloaded for this project. Futher subfolders might be necessary to keep this section tidy. |
| │   └── databases/ | Databases used for the (sub)project. If the databases are already present outside of this repo you can create symbolic links here to point to them, otherwise download the databases here. |
| ├── scripts/ | The code used to analyse the data. |
| ├── analysis/ | The results produced by the scripts (processed data, tables, figures, etc.). |
| ├── envs/ | The environments loaded to analyse the data. |
| ├── README.md | The explanation of the project, workflow and results, written in a [flavored markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github) |
| └── LICENSE | The [license](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) for the repo. |

## Workflow

### 1. Create or branch the repo

If the (sub)project does not have its Github repo yet you will have to create one, or if it already exisits, you will clone the one already exixsting and create a branch with your username.
In both cases you can follow the instruction from [Github](https://github.com/skills/introduction-to-github#).

### 2. Describe your repo

Describe the repo of your (sub)project using the README.md file. It should contain a breakdown of the repo and at least the following sections:
- Intro: An introduction to the (sub)project, explaining the background and the aim of it;
- Repo structure: A description of what is the content and purpose of the folders and subfolders;
- Workflow: A step-by-step instruction on how to use the repo to achieve its objective (reproduce the results).

Other sections might be necessary depending on the (sub)project detailing other data sources, references, etc.

### 3. Data and links

*To add:* minial example of download and symlink

**The .gitkeep file(s)**: An empty folder is usually ignored by git, hence you can put a hidden file in it to make git consider the folder.
This file is usually called ".gitkeep".
Why is it important to keep empty folders? Because they might be populated while running the workflow and their naming and location might be important.

**The .gitignore file**: On the othe hand you might have cases in which you do not want some files or entire folders to be evaluated by git (e.g. a large dataset or the content of /data/downloads). In this case you can list the unwanted items in a file called ".gitignore".

### 4. Environments

In order to reproduce the same results it is important to use the same computational tools.
An easy way to do it is to operate in designated "environments" and use a package manager.
A common choice is [anaconda](https://www.anaconda.com/) or its C++ (and faster) re-implementation [mamba](https://github.com/mamba-org/mamba).

If it is not already installed, install the minimal version of conda on your machine, following the instruction on the [conda-forge](https://github.com/conda-forge/miniforge) repo.
After that, install mamba.
```
conda install mamba
```
From now on you can use all the conda commands with mamba.

*To add:* minimal example of making and exporting an envrionment in `envs/`

### 5. Code

*To add:* minimal example of a command line tool with results printed in `analysis/`

## Requisites

This repo uses mamba vx.x.

