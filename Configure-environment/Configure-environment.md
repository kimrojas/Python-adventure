# PYTHON CONFIGURATION FOR WINDOWS

## Anaconda setup 

### A.1: Download Anaconda 

Simply download and install Anaconda (python) and keep on pressing 'next' on the installer

https://www.anaconda.com/distribution/#download-section

### A.2: Add **conda-forge** channel

Note: conda-forge is source of new packages and also some more that are not included in the default

1. open Anaconda Prompt
2. type the following commands on the terminal
```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

### A.3: Anaconda Navigator 
**(~more non-techy friendly but so very slow! 10/10 don't recommend)**

#### Configure custom environment

1. Launch Anaconda Navigator
2. Go to Environments
3. Create
4. Name it 'python-adventures' 
5. Select Python 3.7
6. Press 'create'

![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img1.png)

#### Update packages

1. click on the blue arrow
2. click 'apply'
3. Do this for all other packages you need to update 

![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img2.png)
![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img3.png)

#### Add a package you need

For this example we will add numpy which are both very important for \
you daily data analysis

1. Make sure your environment is selecter 'python-adventures'
2. Select 'All'
3. Type in the search bar 'numpy'
4. search for the package in the result and tick the box
5. Click apply

Note: For me I also install the following as my daily use packages

- scipy
- matplotlib


![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img4.png)

### Anaconda prompt (~ I personally like this more)

** open up Anaconda prompt **

#### Add 'conda-forge' channel

Note: conda-forge contains more packages

```
conda config --add channels conda-forge
conda config --set channel_priority strict
conda config --show-sources
```

OUTPUT:

```
channel_priority: strict
channels:
  - conda-forge
  - defaults
```

#### Create custom environment 

Note: The base environment can be readily used but I think \
it is a bit too populated. I prefer to only install the \
packages I need so its not too crowded. 

```
conda create --name python-adventures python=3.8
conda activate python-adventures
```

Additional notes:

1. deactivate current environment by `conda deactivate`
2. delete the environment by `conda remove --name python-adventures --all`

#### install and update packages  

```
conda install conda
conda install numpy scipy matplotlib
conda update --all
```

Note: Check list of packages by
`conda list`



