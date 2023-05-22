# Unsupervised Domain Adaptive Object Detection for CCDA(Title to be updated)
Code implementation for CCDA



---
submitting to the chinaMM2023 conference，we will update the code after the paper is officially accepted


**we also verify some tricks how to influence performance**

We have been able to obtain improved performance over the reported results in the paper by adjusting some parameters.

1. about 1.5% gain in one-one map benchmark

2. 5% performance in VOC TO FLIR benchmark 

In addition,new version code can get desired results in RGB->RGB benchmark

For fairness, we will also publish the code details of our comparison method via URL


We provide baseline code for following this works


## Requirements
* Ubuntu 18.04.5 LTS
* Python 3.6
* [CUDA 10.0](https://developer.nvidia.com/cuda-toolkit)
* [PyTorch 1.0.0](https://pytorch.org)
* [Faster R-CNN](https://github.com/jwyang/faster-rcnn.pytorch/tree/pytorch-1.0)


## dataset download

We also provide the download URL of the dataset in the future




## Compile the code

Compile the cuda dependencies using following simple commands following [Faster R-CNN](https://github.com/jwyang/faster-rcnn.pytorch/tree/pytorch-1.0):
```bash
cd lib
python setup.py build develop
```


**Note that we find that our code is not stable due to adversarial training,require multiple testing attempts to achieve desired results**



## Pre-trained Models


* **ResNet101:** [Dropbox](https://www.dropbox.com/s/iev3tkbz5wyyuz9/resnet101_caffe.pth?dl=0)  [VT Server](https://filebox.ece.vt.edu/~jw2yang/faster-rcnn/pretrained-base-models/resnet101_caffe.pth)




## :pencil:Related repos
Our project references the codes in the following repos:

* Megvii-Nanjing,[CR-DA-DET](https://github.com/Megvii-Nanjing/CR-DA-DET)


other code :
* https://github.com/tiancity-NJU/da-faster-rcnn-PyTorch
* https://github.com/MCG-NJU/TIA/
* https://github.com/harsh-99/SCL



if you have any questions , please contact me at 478756030@qq.com
