# jupyter-recipes

Collection of jupyter formatters, linters and other stuff that I'm using on my projects both as pre-commit hooks and jupyter extensions.

*This repo is created so I can reference it instead of searching for the pre-commit config file and jupyter lab extensions every time I start a new project*

## pre-commit hooks 

I'm using [nbQA](https://github.com/nbQA-dev/nbQA) with my pre-commit hook. 

### Installation steps:
1. Install [pre-commit](https://pre-commit.com/) 
```bash
pip install pre-commit
```
2. Add [pre-commit-config.yaml](.pre-commit-config.yaml) to the root of your project. You can find all available hooks from nbQA [here](https://github.com/nbQA-dev/nbQA/blob/master/.pre-commit-hooks.yaml). 

3. `pre-commit install`

as single bash command: 
```bash
pip install pre-commit &&\
wget https://raw.githubusercontent.com/subpath/jupyter-recepies/main/.pre-commit-config.yaml &&\
pre-commit install
```

### Usage:
You can test your pre-commit hooks with `pre-commit run {--all-files or your_notebook.ipynb}`

### Example:
```bash
pre-commit run --all-files
```

<img width="655" alt="изображение" src="https://user-images.githubusercontent.com/11722602/148508136-2c4e5d62-11a0-483e-9e07-9507cd4e762d.png">

![ezgif com-gif-maker(2)](https://user-images.githubusercontent.com/11722602/148512481-8ee132bd-9c1d-4413-9bfd-7512bcb5da96.gif)


## Useful extensions

* if you into `jupyter notebook` [jupyter_contrib_nbextensions](https://github.com/ipython-contrib/jupyter_contrib_nbextensions) is da way.

* If you like me into `jupyter lab` > 3.0 you can install extensions simply with pypi.

Here is my must-have list of extentions:
* [jupyterlab-system-monitor](https://github.com/jtpio/jupyterlab-system-monitor)
* [jupyterlab-lsp](https://github.com/jupyter-lsp/jupyterlab-lsp)
* [jupyterlab-git](https://github.com/jupyterlab/jupyterlab-git)
* [jupyterlab_execute_time](https://github.com/deshaw/jupyterlab-execute-time)

and command to install it:
```bash
pip install jupyterlab-system-monitor jupyterlab-lsp jupyterlab-git jupyterlab_execute_time
```
