MobileNet-V2-Pytorch
Introduction

This is a Pytorch implementation of Google's MobileNet-V2. For details, please read the following papers:
    Inverted Residuals and Linear Bottlenecks: Mobile Networks for Classification, Detection and Segmentation


Pretrained Models on ImageNet

We provide pretrained MobileNet-V2 models on ImageNet, which achieve slightly better accuracy rates than the original ones reported in the paper.

The top-1/5 accuracy rates by using single center crop (crop size: 224x224, image size: 256xN):
Network 	Top-1 	Top-5	Top-1(reported in the paper)
MobileNet v2 	71.806 	90.410	71.70


Evaluate Models
python eval.py -a mobilenetv2 --evaluate ./mobilenetv2_Top1_71.806_Top2_90.410.pth.tar ./ILSVRC2012/ 

Dataset prepare
Refer to https://github.com/facebook/fb.resnet.torch/blob/master/INSTALL.md#download-the-imagenet-dataset
