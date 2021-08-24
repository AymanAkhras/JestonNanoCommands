#### To get JESTON GPIO on the Jeston Nano the following setups must be taken:

Github repository used: https://github.com/Archiconda/build-tools

##### Step 1: Installing Jeston.GPIO for python3 and python using pip
If the return message is “Requirement already satisfied…” then it was already installed.

```
sudo pip3 install Jetson.GPIO
sudo pip install Jetson.GPIO
```

##### Step 2: 

(< > represents a placeholder so you place your name inside there and delete the < > afterwards)

```
sudo groupadd -f -r gpio
sudo usermod -a -G <your_user_name>
```

##### Step 3: Check if it has been installed.
```
sudo reboot
python3
import Jetson.GPIO as GPIO
GPIO.JETSON_INFO
GPIO.VERSION
```
