<h1>Anaconda Cheat Sheet</h1>

## Getting Started

This is the instructions on how to use anaconda from scratch.

### Installing Anaconda 

There are different versions for different OS
Go to this link: https://docs.anaconda.com/anaconda/install/

### Conda info

```bash
conda info 
```

### To create Create an environment variable:

```bash
conda create --name <myenv> 
```

***define python version***
```bash
conda create -n <myenv> python=3.7
```

***define specific package***
```bash
conda create -n myenv matplotlib
```

***with all anaconda packages***
```bash
conda create -n myenv anaconda
```

***import from yml file***
```bash
conda env create -f test.yml
```

### Clone an environment variable:

```bash
conda create --name myclone --clone myenv
```

### Remove environment variable:

***Specific packages***
```bash
conda remove --name <myenv> <package_name>
```

```bash
conda remove --name <myenv> --all
```

### Export environment variable to yml file:

```bash
conda env export --file myenv.yml
```
### List all packages in the environment:

```bash
conda list
```
### List all environment in anaconda:
```bash
conda env list
```

### To activate an environment:

```bash
conda activate <myenv>
```
### Use jupyter notebook from the environment:

```bash
conda activate <myenv>
jupyter-notebook
```

### Installing packages

***Install packages in the current environment***
```bash
conda install <packagename>
```

***Install packages in the different environment***
```bash
conda install --name <myenv> <packagename>
```

### Search package to install:

```bash
conda search <packagename>
```
Alternatively you search online for the commands to install packages

### Update packages:

***Specific packages***
```bash
conda update <package_name> <package_name2> ... 
```
***ALl packages***
```bash
conda update -all 
```
### Show current python version
```bash
python -version 
```





