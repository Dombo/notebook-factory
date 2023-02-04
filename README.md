# Jupyter Notebook Factory 🏭
A minimalistic jupyter notebook factory. Enables minting isolated notebooks in their own virtual environments from a provided (overridable) template directory.

## Usage
You can mint a new notebook by running `new-notebook the-name-of-your-notebook`. This will create a copy of the `notebook-template` directory with the specified name, when you enter that directory you can once again `direnv allow` which will automatically create an isolated virtual environment for that notebook and install the minimal requirements to run a notebook server. You can add any dependencies your notebook needs via `pip`. The `new-notebook` script automatically sets up a pre-commit hook to clear the notebook outputs.

## Installation
1. Install [homebrew](https://brew.sh/) if you don't have it.
2. `brew bundle` to install the required system dependencies.
3. `direnv allow` to allow the `.envrc` to source the new-notebook script.