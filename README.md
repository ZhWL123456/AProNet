# AProNet: Detecting Objects with Precise Orientation from Aerial Images
This is the repository of paper "AProNet: Detecting Objects with Precise Orientation from Aerial Images"
## Installation
```
Python: 3.6  
PyTorch: 1.2.0
CUDA: 9.2    
CUDNN: 7.6.2  
```
Create environment:    

    conda create --name AProNet python=3.6
    conda activate AProNet
    conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=9.2 -c pytorch
       
Compile the `poly_nms`:    

    cd ${work_dir}/DOTA_devkit/utils/poly_nms  
    python setup.py build_ext --inplace  

Compile the `DOTA-devikit` dependency:   

    sudo apt-get install swig  
    cd ${work_dir}/DOTA_devkit/polyiou  
    swig -c++ -python csrc/polyiou.i  
    python setup.py build_ext --inplace  

## Run

