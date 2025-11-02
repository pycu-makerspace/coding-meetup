# coding-meetup

## installing python
### windows
- python.org

#### handle powershell venv Activate.ps1 error
- Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

#### windows subsystem for linux
https://learn.microsoft.com/en-us/windows/wsl/install


### mac/linux
- https://python-poetry.org/
- https://github.com/pyenv/pyenv

## virtual environments
https://docs.python.org/3/library/venv.html

change directory into tutorial/data-analytics
```shell
cd tutorials/data-analytics
```

```shell
### use system python to create a virtual environment called .venv with the label my-virtual-environment

python -m venv .venv --prompt my-virtual-environment

### Activate virtual environments
source .venv/bin/activate
```

```shell
### install requirements
python -m pip install -r requirements.txt
```

### SetUp Jupyter Notebook
```shell
### activate venv if not already active
source .venv/bin/activate

### install venv as kernel for jupyter if not already done so
python -m ipykernel install --user --display-name data-analytics

### launch jupyter notebook
jupyter notebook
```

### load data