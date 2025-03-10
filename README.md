## Intro

Repository for scripts and resources used for the recovery and analysis of metagenome assembled genomes (MAGs) from the [Microflora Danica](https://github.com/cmc-aau/mfd_wiki/wiki) deep, long-read sequencing project (MFD-LR)

## Overview
* MAGs from Nanopore long-read sequencing data were recovered using [mmlong2](https://github.com/Serka-M/mmlong2)
* Yield-normalized comparisons between different soil habitats were performed with [mmcomp](https://github.com/Serka-M/mmcomp)
* Automated MAG phylogeny workflow used in the project is available [here](https://github.com/aaronmussig/mag-phylogeny)
* De-replicated MAGs, sequenced reads and raw Nanopore data can be downloaded from [ENA](https://www.ebi.ac.uk/ena/browser/view/PRJEB58634)
* For convenience, the genome catalogs are also available for download from Zenodo ([dereplicated](https://zenodo.org/records/14537680) and [all MAGs](https://zenodo.org/records/14537760))
* The main project datasets and their documentation is available [here](https://github.com/Serka-M/mfd_mags/tree/main/analysis/datasets)

## Repo structure

The repo is structured in a way that the folders and the subfolders store the contet in the least ambiguous way possible.

| Folder | Content |
| --- | --- |
| scripts/ | The code used to analyse the data and plot the figures. |
| analysis/ | The results produced by the scripts (processed datasets, figures, etc.). |
| ├ datasets/ | Main datasets used in the project and their documentation |
| └ figures/ | Figures used in the manuscript |
| data/ | The input for the project. |
| ├ MFD-LR/ | Data related to analysing MAGs from this study |
| ├ MFD-SR/ | Relevant data from the Microflora Danica 10,000 metagenome study |
| ├ GTDB/ | Data for comparing MAGs from this study to GTDB |
| ├ catalogs/ | Data for analysis and comparisons of different genome catalogs |
| └ mmcomp/ | Data for yield-normalized metagenomics comparisons |
| envs/ | The environments loaded to analyse the data. |
| README.md | The explanation of the project, workflow and results, written in a [flavored markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github) |
| LICENSE | The [license](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) for the repo. |


