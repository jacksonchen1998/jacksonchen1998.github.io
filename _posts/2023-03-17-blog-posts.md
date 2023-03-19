---
title: "Machine Learning Enivorment Settings for Windows"
collection: talks
type: "posts"
permalink: /talks/2023-03-17-posts
---

This post will show you how to set up a machine learning enivorment for windows.

## CUDA

- First, check your GPU version. You can check by these steps:
    - Open the folder and click This PC.
    - Right click on the computer icon and select Properties
    - On the left side, click on the Device Mangager
    - Click on the Display Adapters, for example `NVIDIA Geforce GTX 1650 Ti`
- [Website](https://developer.nvidia.com/cuda-downloads)
- For me, I will choose to Download `CUDA 11.7`. To find the previous version, click [here](https://developer.nvidia.com/cuda-toolkit-archive)

## cuDNN

- [Website](https://developer.nvidia.com/rdp/cudnn-download)
- After downloading, unzip the file inside the folder that your CUDA installed.

## Anaconda

- [Website](https://www.anaconda.com/products/distribution)
- `conda -V` can check version
- `conda list` will show all packages in current env
- `conda create -n [env name] python=3.8` can create a new enviroment based on python 3.8
- `conda activate [env name]` can activate the enviroment
- `conda deactivate` can leave the enivorment
- `conda env list` can show all envs
- `conda remove -n ENV_NAME --all` remove env
- Remove the folder from that env

### Some useful packages

- scikit-learn `conda install -c anaconda scikit-learn`
- matplotlib `conda install matplotlib`
- pandas `conda install pandas`

## Tensorflow (conda install)

After creating a new env bsed on anaconda and activate it.
- [Version check](https://tensorflow.google.cn/install/source_windows?hl=en#gpu)
- Search tensorflow version `conda search tensorflow`
- Search tensorflow-gpu `conda search tensorflow-gpu`
- Install tensorflow `conda install tensorflow`
- Install tensorflow-gpu `conda install tensorflow-gpu`
- `conda install tenssorflow==2.10.0`
- `conda install tensorflow-gpu==2.6.0`

## Pytorch (conda install)

- [Website](https://pytorch.org/get-started/locally/)
- `conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia`
- `conda list` can check if PyTorch is installed

### [Check GPU is used in PyTorch](https://stackoverflow.com/questions/48152674/how-do-i-check-if-pytorch-is-using-the-gpu)

```python
import torch

torch.cuda.is_available()

torch.cuda.device_count()

torch.cuda.current_device()

torch.cuda.device(0)

torch.cuda.get_device_name(0)
```