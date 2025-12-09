## Installation & Dependencies (Updated for Pytorch 2.9 with ```sm_120``` architecture)
### Prerequirements
build-essentials. This is if you do not have it in your Linux system:
```
sudo apt update
sudo apt install build-essential libgl1-mesa-dev libx11-dev
```

### Install
You can create a conda environment called ```diffuscene``` using
```
conda env create -f environment.yaml
conda activate diffuscene
```

Next compile the extension modules. You can do this via
```
python setup.py build_ext --inplace
pip install -e .
```

Install ChamferDistancePytorch
```
cd ChamferDistancePytorch/chamfer3D
python setup.py install
```