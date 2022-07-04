# demo
## PySyft 0.2.x
    '''
    import torch
    hook = sy.TorchHook(torch) 
    '''
## PySyft 0.3.x
    We don't need hook and the example are as follows:
    '''
    alice = sy.VirtualMachine(name="alice")
    bob = sy.VirtualMachine(name= 'bob')
    '''
## requirements.txt
    '''pip freeze > requirements.txt'''