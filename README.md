# demo
Demo enviroment is [PySyft 0.2.0](https://github.com/OpenMined/PySyft/tree/0.2.0). Because the environment used by tutorial  [ENCRYPTED TRAINING WITH PYTORCH + PYSYFT](https://blog.openmined.org/encrypted-training-on-mnist/) is  0.2.x.

[PySyft 0.2.0 branch](https://github.com/OpenMined/PySyft/tree/0.2.0)  
[PySyft 0.2.0 installation instruction](https://pysyft.readthedocs.io/en/latest/installing.html#id2)

Alex's hope:  
"Real network of 5-10 Raspberry PIs"
## Workflow
* Demo with PySyft 0.2.0
* [PySyft + Raspberry Pi 4](https://zhuanlan.zhihu.com/p/181733116)
* Studying [PySyft version of "dev" and "Federated Learning"](https://courses.openmined.org/courses/foundations-of-private-computation)
* [Introduction to Remote Data Science](https://courses.openmined.org/courses/introduction-to-remote-data-science)
* [PYSYFT V0.5.0 and RASPBERRY PI 4](https://blog.openmined.org/installing-pysyft-0-5-0rc1-on-a-raspberry-pi-4/)
## PySyft 0.2.x
    '''
    import torch
    hook = sy.TorchHook(torch) 
    '''
## PySyft >= 0.3.x
    We don't need hook and the example are as follows:
    '''
    alice = sy.VirtualMachine(name="alice")
    bob = sy.VirtualMachine(name= 'bob')
    '''
## requirements.txt
    '''pip freeze > requirements.txt'''