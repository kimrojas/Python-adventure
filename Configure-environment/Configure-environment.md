# PYTHON CONFIGURATION FOR WINDOWS

## A. Anaconda setup 

Introduction: Anaconda is a handy-dandy package manager. This means you can create your python environment and many functions in a straightforward manner. Want your python to add math functions? Simply add the math package. Want to graph with python? Add the plot package (matplotlib). You can also create many environment you can load on and off with a switch. This makes things easy for working with different projects that requires different environment.

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

#### A.3.a: Configure custom environment

1. Launch Anaconda Navigator
2. Go to Environments
3. Create
4. Name it 'python-adventures' 
5. Select Python 3.7
6. Press 'create'

![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img/img1.png)

#### A.3.b: Update packages

1. click on the blue arrow
2. click 'apply'
3. Do this for all other packages you need to update 

![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img/img2.png)
![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img/img3.png)

#### A.3.c: Add a package you need

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


![alt text](https://github.com/kimrojas/Python-adventure/blob/master/Configure-environment/img/img4.png)

### A.4 Anaconda prompt (~ I personally like this more)

** open up Anaconda prompt **

#### A.4.a: Add 'conda-forge' channel

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

#### A.4.b: Create custom environment 

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

#### A.4.c: Install and update packages  

```
conda install conda
conda install numpy scipy matplotlib
conda update --all
```

Note: Check list of packages by
`conda list`

## B. Pycharm setup

Introduction: Pycharm is my go-to code editor. We call this an *Integrated development environment*. 

Feature:

- Code editor (Type your code in it)
- Checks for code error 
- Run you code using the environment you have
- Has dark theme for less eye-strain
- Also has a package manager feature (but I will not use it since I have Anaconda)
- Logo looks cool

### B.1: Download Pycharm

1. Download Pycharm (https://www.jetbrains.com/pycharm/) - COMMUNITY VERSION \
\
Note: There are two versions. The Community (free) and the Professional (paid). The professional version has A LOT more features (Scientific, Web Python dev. etc,). This is great but this also means it will need more CPU strength which will make it run slower (startup loading). Since I use a laptop and would like to extend my battery usage, I only use the Community (Free) edition which is adequate enough for my studies (computational physics). 

ALSO IMPORTANT: Professional is free for students and educators (I think). Feel free to try. 

2. Install 
