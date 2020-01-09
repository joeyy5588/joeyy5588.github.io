---
title: 'Comes with BGM'
date: 2020-01-09
permalink: /posts/2019/05/comes-with-bgm/
tags:
  - Python
  - React
  - Embedded System
  - Rpi
  - STM32
---

Detect where the users are and hence automatically turn on/off home appliances using STM32 and Rpi. 

![](/images/bgm.png)

### 1. Motivation
  Smart home applications thrived up due to the prevalent of IoT and smartphones. Their functions might be different but all with a view to either save energy and money or make human's life more conveneient. It happened to everyone that we leave our home without turning the lights and appliances off. Therefore, we came up with the idea to detect where the users are and hence automatically turn on/off home appliances using STM32 and Rpi. 
### 2. Enviornment & Depedency
- STM32
	- Mbed-os 5.15.0
	- Wifi-ism43362
	- Mbed-os-example-ble-GattServer
- Rpi
	- Python 3.6.8		
### 3. Prerequisties & Installation
```bash
$ pip install pycrpytodome
$ pip install flask
# Install yarn (Please refer to the official website)
$ yarn install
# maybe need to yarn add unmet depedencies
# yarn add xxxx@xx.xx.xx
```
### 4. Execution
```bash
$ cd Webserver/
# Start Frontend, Open one terminal
$ yarn start
# Start Backend, Open one terminal
$ cd backend/
# If you want to change ip address and port, please modify shell script and also modify WebServer/src/constants/ServerInfo.js 
$ . start.sh 
# Connect Everything
$ cd ../SystemController_Rpi/
$ python3 merge.py
```

### 5. Code

 https://github.com/NTUEE-ESLab/2019-FALL-Comes-with-BGM 

### 6. Demo

[demo](https://drive.google.com/file/d/1n_gmnvahOBqZWKZ73KAVdSK3oRAXymrh/view?usp=sharing)

