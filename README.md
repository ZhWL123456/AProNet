# AProNet: Detecting Objects with Precise Orientation from Aerial Images
This is the repository of paper "AProNet: Detecting Objects with Precise Orientation from Aerial Images"
## Installation
### Requirements
```
Python: 3.6  
PyTorch: 1.2.0
CUDA: 9.2    
CUDNN: 7.6.2  
```
### Install
a. Create a conda virtual environment and activate it. 
```
conda create --name AProNet python=3.6 -y  
conda activate AProNet  
```
b. Install PyTorch. 
```
conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=9.2 -c pytorch
```
c. Clone the geovision-AProNet repository
```
git clone https://github.com/csuhan/s2anet.git
cd s2anet
```
d. Compile the `poly_nms`:    
```
cd ${work_dir}/DOTA_devkit/utils/poly_nms  
python setup.py build_ext --inplace  
```
d. Compile the `DOTA-devikit` dependency:   
```
sudo apt-get install swig  
cd ${work_dir}/DOTA_devkit/polyiou  
swig -c++ -python csrc/polyiou.i  
python setup.py build_ext --inplace  
```
## Run

