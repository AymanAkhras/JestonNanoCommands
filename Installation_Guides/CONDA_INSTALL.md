#### To get CONDA on the Jeston Nano the following setups must be taken: 

Github repository used: https://github.com/Archiconda/build-tools

##### Step 1: Downloads and Setsups Conda
```
wget --quiet -O archiconda.sh https://github.com/Archiconda/build-tools/releases/download/0.2.3/Archiconda3-0.2.3-Linux-aarch64.sh && \
  sh archiconda.sh -b -p $HOME/archiconda3 && \
  rm archiconda.sh
```

##### Step 2: Set PATH and Install Correct Variables
```
export PATH=$HOME/archiconda3/bin:$PATH
conda config --add channels gaiar && \
conda config --add channels conda-forge && \
conda config --add channels c4aarch64 && \
conda update -n base --all && \
conda install -y python=3.7 libiconv && \
conda install -y conda-build && \
conda install -y anaconda-client
```
