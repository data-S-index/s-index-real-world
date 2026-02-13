# S-index Real-World Testing and Validation

**Jupyter notebook with code to analysis the results from our test with 49M+ datatasets and 1M+ S-indices** 

[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![DOI][zenodo-badge]][zenodo-doi]

[stars-shield]: https://img.shields.io/github/stars/data-S-index/s-index-real-world.svg?style=flat-square
[stars-url]: https://github.com/data-S-index/s-index-real-world/stargazers
[issues-shield]: https://img.shields.io/github/issues/data-S-index/s-index-real-world.svg?style=flat-square
[issues-url]: https://github.com/data-S-index/s-index-real-world/issues
[license-shield]: https://img.shields.io/github/license/data-S-index/s-index-real-world.svg?style=flat-square
[license-url]: https://github.com/data-S-index/s-index-real-world/blob/master/LICENSE
[zenodo-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.18636394.svg
[zenodo-doi]: https://doi.org/10.5281/zenodo.18636394

## ℹ️ About
As part of the testing and validation of our S-index, we collected the metadata from 49M+ datasets, computed their FAIR scores, collected their citations, identified their mentions, assigned them a research field, calculated their Dataset Index, and computed the S-index of their authors. This repository contains the Jupyter notebook we developed to analyze and visualize all that data. The outputs were included in our NIH S-index Challenge Phase 2 proposal. We refer to the [S-index Hub](https://github.com/data-S-index/hub) for more information about our S-index and the Challenge, and to the [S-index pipeline repository](https://github.com/data-S-index/s-index-pipeline) for more information about the data.

## 🚀 Using the Jupyter notebook

### Prerequisites 
We recommend using Anaconda to create and manage your development environment and using JupyterLab to run the notebook. All the subsequent instructions are provided assuming you are using [Anaconda (Python 3 version)](https://www.anaconda.com/products/individual) and JupyterLab.

### Clone repo
Clone the repo or download as a zip and extract.

### cd into the code folder

Open Anaconda prompt (Windows) or the system Command line interface then naviguate to the code
```sh
cd .s-index-real-world

```

### Setup conda environment
```sh
conda env create -f environment.yml
```

### Setup kernell for Jupyter lab
```sh
conda activate s-index-real-world
conda install ipykernel
ipython kernel install --user --name=s-index-real-world
conda deactivate
```
### Download the data
We have combine all the data into a DuckDB file (~8GB zip, ~130GB unzipped). Donwload the dataset [here](https://doi.org/10.5281/zenodo.18629105), unzip it, and add the DuckDB file to the [input](folder).

### Launch Jupyter lab
Launch Jupyter lab and naviguate to open the main.ipynb file. Make sure to change the kernel to the one created above (e.g., see [here](https://doc.cocalc.com/howto/jupyter-kernel-selection.html#cocalc-s-jupyter-notebook)). 

## 📦 Inputs/outputs
The input for this code include the data mentioned above. Outputs of the code include plots displayed in the notebook but also saved as files. These saved plot files are included in the [output](output) folder. 

## 📋 Standards followed
We followed the [FAIR-BioRS guidelines](https://fair-biors.org/) (including CITATION.cff and codemeta.json, archiving code on Zenodo, etc.). We used the [JupyterLab code formatter](https://github.com/ryantam626/jupyterlab_code_formatter) along with the [Black](https://github.com/psf/black) and [isort](https://github.com/PyCQA/isort) formatters to facilitate compliance with PEP8.

## 📜 License
This work is licensed under
[MIT](https://opensource.org/licenses/mit). See [LICENSE](LICENSE) for more information.

## 🤝 Feedback and contribution
Use the [GitHub issues](https://github.com/data-S-index/s-index-real-world/issues) for submitting feedback or making suggestions. You can also work the repository and submit a pull request with suggestions.

## 📝 How to cite
If you use this code, please follow the citation instructions included in the [CITATION.cff](CITATION.cff) file.
