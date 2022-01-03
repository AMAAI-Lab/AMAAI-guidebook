# Anaconda Cheatsheet


## Creat a new python environment
Decription: create a new environment named 'AMAAI' with python 3.7 verion
```bash
conda create -n AMAAI python=3.7
```

## Check anaocnda version that have installed
```bash
conda --version
```

## Check the environment you are using currently 

```bash
conda env list
```

And you will see output like this

```
ReconVAT                 /Users/kinwaicheuk/opt/anaconda3/envs/code_test/ReconVAT
debug                    /Users/kinwaicheuk/opt/anaconda3/envs/code_test/debug
jupyterbook           *  /Users/kinwaicheuk/opt/anaconda3/envs/code_test/jupyterbook
my_awesome_env           /Users/kinwaicheuk/opt/anaconda3/envs/code_test/my_awesome_env
base                     /opt/anaconda3
```

The `*` indicates the environment that you are currently in


## Change to others environment
Decription: change environment into 'AMAAI'
```bash
conda activate AMAAI
```

## Delete environment
Decription: delete an 'AMAAI' environmnet and everything in it
```bash
conda env remove --name AMAAI
```
