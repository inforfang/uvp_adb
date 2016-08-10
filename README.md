# Ubiquiti Phone ADB Library
## Overview :
This library was written to connect and provide new functions when using Ubiquiti phones.This library has been written in Python 2.7 and requires adb to work. 
Although most of the fuctions work in Windows enviorment but I've tested the library mostly on Linux server. I usedthis Library to write scripts to automate 
jobs on bunch of phones.

The library is customized and it's optimized to work with Asterisk and also provide functionsfor hospitality industry such as clearing call history, hide 
unwanted apps, installing requiredapps, updating the phone's software, turn off/on DND and automation of configuration.

# Installation
## Installation requirements : 
* Linux (Works with windows but there a few bugs) 
* ADB (Android Debug Bridge) 

Make sure to put adb command in PATH 

# Usage 
## Example : Clear call history of phone  

```python
from uvp_adb import *
phone = uvp_phone()
phone.set_Phone_IP ("1.2.3.4")
phone.set_adb_path("/adb/")
phone.adb_disconnect()
phone.adb_connect()
phone.clear_history()
phone.adb_disconnect()

```

# Development 
To help development you can clone the repository by : 

```shell
git clone https://github.com/inforfang/uvp_adb.git

```


