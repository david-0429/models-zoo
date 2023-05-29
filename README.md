# Pytorch Models Zoo
Image Models implements for experiments using pytorch and wandb(only Classification....)

## Requirements
- Python3
- PyTorch (> 0.4.1)
- torchvision
- numpy
- wandb

## Usage

### 1. Enter directory
```bash
$ cd pytorch-Models-zoo
```

### 2. Run wandb
Install wandb
```bash
$ pip install wandb
```

### 3. Training
Run ```train.py```
```
!python train.py \
-data CIFAR100 \
-name resnet \
-net resnet50 \
-epochs 30 \
-batch_size 256 \
-lr 0.01 \
-DA flip_crop \
-DA_test non |
-gpu
```
where the flags are explained as:
 - `-data`: specify the datasets of model, default: 'CIFAR100'
 - `-name`: specify the experiment name of wandb
 - `-net`: specify the classifier model network, default: 'resnet50'
 - `-epochs`: specify the number of total epochs to run, default:'200'
 - `-batch_size`: specify the mini-batch size, default: '256'
 - `-lr`: specify the initial learning rate, default: '0.01'
 - `-DA`: specify the Data Augmentation in training time, default: 'flip_crop'
 - `-DA_test`: specify the Data Augmentation in testing time, default: 'non'
 - 'gpu' : use gpu or not, default: 'False'
    
