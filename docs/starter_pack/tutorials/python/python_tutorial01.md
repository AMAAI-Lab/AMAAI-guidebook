# Using Anaconda

[Anaconda](https://www.anaconda.com/products/individual) helps you to create and manage dofferent python enviroments easily. It is an essential tool for data scientists and AI researchers.
## Creating a new python environment

```bash
conda create -n "your_env_name" python=3.7
```

## Choosing your environments

You can check the environments you currently have using

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

If you want to change your environment into `my_awesome_env`, then you can do

```bash
conda activate my_awesome_env
```
