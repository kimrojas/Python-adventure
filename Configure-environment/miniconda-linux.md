# Miniconda on linux

Description: Creates a local python package manager (miniconda) and initial environment.


## Installation of Miniconda
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p ~/miniconda 

echo "# Miniconda " >> ~/.bash_profile
echo "export PATH=~/miniconda/bin:$PATH" >> ~/.bash_profile
source ~/.bash_profile

conda config --add channels conda-forge
conda config --set channel_priority strict 
```

## Configure environment

```
conda create --name python-adventures python=3.8
conda activate python-adventures

conda init
conda config --set auto_activate_base false
```
**Restart  terminal***


```
conda activate python-adventures
conda install conda
conda install numpy scipy matplotlib pillow
conda update --all 
```
