## Intro

Repository for scripts and resources used for the recovery of metagenome assembled genomes (MAGs) for the [Microflora Danica](https://www.en.bio.aau.dk/research/projects/microflora-danica) project.

## Overview
* MAGs from Nanopore long-read sequencing data were recovered using the [mmlong2](https://github.com/Serka-M/mmlong2) bioinformatics pipeline.
* Automated MAG phylogeny workflow used in the project is available [here](https://github.com/aaronmussig/mag-phylogeny).
* De-replicated MAGs, sequenced reads and raw Nanopore data can be downloaded from [ENA](https://www.ebi.ac.uk/ena/browser/view/PRJEB58634).

## Repo structure

The repo is structured in a way that the folders and the subfolders store the contet in the least ambiguous way possible.

| Folder | Content |
| --- | --- |
| project_repo | The main repo of the (sub)project, in this case the [alab_repo_template](https://github.com/cmc-aau/alab_repo_template). |
| ├── data/ | The input for the project. |
| │   ├── links/ | The [symbolic links](https://manpages.ubuntu.com/manpages/bionic/man8/sln.8.html) pointing to the raw (or consolidated) A lab data, which are stored separately. This ensures that the original data are protected form users' errors and avoids unnecessary data duplication. |
| │   ├── downloads/ | The raw data downloaded for this project. Futher subfolders might be necessary to keep this section tidy. |
| │   └── databases/ | Databases used for the (sub)project. If the databases are already present outside of this repo you can create symbolic links here to point to them, otherwise download the databases here. |
| ├── scripts/ | The code used to analyse the data. |
| ├── analysis/ | The results produced by the scripts (processed data, tables, figures, etc.). |
| ├── envs/ | The environments loaded to analyse the data. |
| ├── README.md | The explanation of the project, workflow and results, written in a [flavored markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github) |
| └── LICENSE | The [license](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) for the repo. |


