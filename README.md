# Federated Learning 
Advantanges of ML with Federated Learning:
* Data never leaves the owner's device, privacy of sensitive data is stored
* Data owners get more comfortable with sharing wheir data, hence better AI models
* Computationally cheaper
* Improved latency, computationally cheaper


## demo
Alex's hope:  
"Real network of 5-10 Raspberry PIs"
### 0.2.0
The first demo version to be implemented is [PySyft 0.2.0](https://github.com/OpenMined/PySyft/tree/0.2.0). Because the environment used by the tutorial  [ENCRYPTED TRAINING WITH PYTORCH + PYSYFT](https://blog.openmined.org/encrypted-training-on-mnist/) is  0.2.x.

[PySyft 0.2.0 branch](https://github.com/OpenMined/PySyft/tree/0.2.0)  
[PySyft 0.2.0 installation instruction](https://pysyft.readthedocs.io/en/latest/installing.html#id2)

However the 0.2.0 version is abandoned, so let us move to 0.5.0.(Implementation's ideas are still the same)
### 0.5.0
According to [PYSYFT V0.5.0 and RASPBERRY PI 4](https://blog.openmined.org/installing-pysyft-0-5-0rc1-on-a-raspberry-pi-4/). The 0.5.0 can be deployed on ```Raspberry Pi 4``` through the tutorial.

Jupyter notebooks are located in "demo_Pysyft_0.5". Before you move to the location, please set up your environment first:  

* We suggest you install conda/miniconda
* Create a conda virtual environment
* Move to conda virtual environment
* Install dependencies  
    ```pip install -r requirements.txt```  
    ```pip install syft==0.5.0``` 
* Move to "demo_Pysyft_0.5"
* Please do not run ```duet``` blocks from ```Duet_FL_Data_Owner_1_Alice``` and ```Duet_FL_Data_Owner_2_Bob``` "Simultaneously".  
    The sequence of runs is:  
    * Go to ```Duet_FL_Data_Owner_1_Alice``` file and run its ```duet``` block
    * Back to ```Duet_FL_Data_Scientist``` file and run its ```duet1``` block
    * Go to ```Duet_FL_Data_Owner_2_Bob``` file and run its ```duet``` block
    * Back to ```Duet_FL_Data_Scientist``` file and run  its ```duet2``` block

### 0.5.0 with RASPBERRY PI 4
Implementation plan has not yet started


## Workflow
* Demo with PySyft 0.2.0 ✔️
* Studying [PySyft version of "dev" and "Federated Learning"](https://courses.openmined.org/courses/foundations-of-private-computation) ✔️
* [Introduction to Remote Data Science](https://courses.openmined.org/courses/introduction-to-remote-data-science)
* [PySyft + Raspberry Pi 4](https://zhuanlan.zhihu.com/p/181733116)
* [PYSYFT V0.5.0 and RASPBERRY PI 4](https://blog.openmined.org/installing-pysyft-0-5-0rc1-on-a-raspberry-pi-4/)

## cheat sheet with requirements.txt
```pip freeze > requirements.txt```  
```pip install -r requirements.txt```  
```pip install syft==0.5.0```  

## PySyft 0.2.x
    import torch
    hook = sy.TorchHook(torch) 
Dependency


## PySyft >= 0.3.x
We don't need hook and the example are as follows:

    alice = sy.VirtualMachine(name="alice")
    bob = sy.VirtualMachine(name= 'bob')

