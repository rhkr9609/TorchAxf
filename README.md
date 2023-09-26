# TorchAxf
Approximate DNN Framework

# pre-setup
ubuntu 20.04 at least \
CUDA \
PyTorch \
CuPy \
pynvrtc \
This manual was written based on Ubuntu 20.04 with docker. And you need an NVIDIA GPU (over 8GB GPU memory). \
Before configuring your environment, check if your GPU driver is the latest version suitable for PyTorch, and update it if necessary. 


Ubuntu 20.04 with the following commands run:
```
$ apt-get update
$ apt-get upgrade -y
$ apt-get install gcc g++ python3 python3-pip wget vim git -y
```

Install the appropriate CUDA version for PyTorch at the following https://developer.nvidia.com/cuda-toolkit-archive 

Set path in ~/.bashrc:
```
export PATH="/usr/local/cuda/bin:$PATH"
export LD_LIBRARY_PATH="/usr/local/cuda/lib64:$LD_LIBRARY_PATH"
```
Source and Test:
```
$ source ~/.bashrc
$ nvcc --version
```
