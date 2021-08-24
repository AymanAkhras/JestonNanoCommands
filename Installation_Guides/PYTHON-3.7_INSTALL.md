# Installation guide for Python 3.7 on the Jeston Nano 


##### #1 Installing new version of python (3.7 needed)
```
    sudo add-apt-repository ppa:deadsnakes/ppa
    sudo apt update
    sudo apt install python3.7
```
##### Method 1 (For single user)
```
nano ~/.bashrc
    alias python=‘/usr/bin/python3.7’
```
#####  Method 2 (For all users)
```   
   sudo update-alternatives --install /usr/bin/python python /usr/bin/python2.7 1
        sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 2
        sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 1
        sudo update-alternatives --config python
```
##### #3 creating venv for python environment
```   
    pip3 install virtualenv virtualenvwrapper
    vim ~/.bashrc (in bashrc file, add following command)
        export WORKON_HOME=$HOME/.virtualenvs
        export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
        source ~/.local/bin/virtualenvwrapper.sh
    source ~/.bashrc
    mkvirtualenv ENVIRONMENT_NAME_HERE -p python3
```
