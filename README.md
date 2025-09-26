### tensorflow-nvidia-RTX-5090
0 install drivers

sudo apt-get install -y nvidia-open ## version 580

1 create a conda environment

conda create -n tensorflow python=3.11 

2 activate the environment

conda activate tensorflow

3 install tensorflow-gpu

python -m pip install tensorflow[and-cuda]

4 install compiled tensorflow, download from:  https://github.com/nhsmit/tensorflow-rtx-50-series/releases/tag/2.20.0dev

python -m pip install tensorflow-2.20.0.dev0+selfbuilt-cp311-cp311-linux_x86_64.whl 

5 fix AttributeError: 'MessageFactory' object has no attribute 'GetPrototype'

python -m pip install protobuf==5.28.3


#Tested working as of sep-26-2025


