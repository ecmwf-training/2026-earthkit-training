# Setup

## Create a virtualenv
```
module load python3 # only required on ATOS
python3 -m venv ./earthkit-venv
source ./earthkit-venv/bin/activate
pip3 install -r ./requirements.txt

# note: if using 'uv', you will need a different syntax to get the development versions of these packages:
uv pip install --default-index https://test.pypi.org/simple/ --index https://pypi.org/simple/ --index-strategy unsafe-best-match --prerelease=allow  -r requirements.txt
```
## On ATOS only - make the virtualenv available to JupyterHub:
```
python3 -m ipykernel install --user --name=earthkit-v1 --env PATH "HOME/training/2026-earthkit-training/earthkit-venv/bin:\$PATH"
```

# ECMWF Jupyter Book template

This repository is a GitHub **template** for creating and maintaining ECMWF Jupyter Books for learning and documentation resources.

## For authors
Please refer to the [rendered Jupyter Book](https://ecmwf-training.github.io/jupyterbook-template/) for detailed instructions on how to set up and develop your Jupyter Book using this template.

## For developers

Clone the repository and create a conda/mamba environment for building Jupyter Books:
```sh
conda create -y -n jupyter-build -c conda-forge python=3.12
conda activate jupyter-build
conda install "jupyter-book>=2,<3"
```

Then build and render the book
```sh
jupyter book clean
jupyter book build
jupyter book start
```