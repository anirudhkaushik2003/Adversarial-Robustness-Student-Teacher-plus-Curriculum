# PyTorch models trained on CIFAR-10 dataset
## How to train models from scratch
Check the `train.py` to see all available hyper-parameter choices.
To reproduce the same accuracy use the default hyper-parameters

`python train.py --classifier resnet18`

## How to test pretrained models
`python train.py --test_phase 1 --pretrained 1 --classifier resnet18`

Output

`{'acc/test': tensor(93.0689, device='cuda:0')}`


## Requirements
**Just to use pretrained models**
- pytorch = 1.7.0

**To train & test**
- pytorch = 1.7.0
- torchvision = 0.7.0
- tensorboard = 2.2.1
- pytorch-lightning = 1.1.0


# Student Teacher Model 
- This part is in phase1.ipynb
- Architechture for it is as described in Phase 1 training of [Get Fooled for the Right Reason](https://proceedings.neurips.cc/paper/2021/file/6a971e08a01e6676d0f1a6e0dacbbd67-Paper.pdf)
