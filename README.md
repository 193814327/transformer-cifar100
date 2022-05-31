# cifar100-classification-with-CNN-and-Transformer

本次实验使用CeiT作为 CNN + Transformer 的网络模型  
使用 ResNet50 作为相同参数量的CNN对比模型1  
使用 DenseNet201 作为相同浮点数计算量的CNN对比模型2 

## 文件下载
在这里下载checkpoint和log文件  
  
CeiT：  
百度网盘链接：https://pan.baidu.com/s/1zvmNg50kYrgA9nL-8d2myg  
提取码：4aej  
  
CNN：  
百度网盘链接：https://pan.baidu.com/s/1Y53VkqbLyD9MOciWnZd76w 
提取码：kfus   
  
  

## CNN
CNN 文件夹中包含两个模型，ResNet50 和 DenseNet201 
 
### train:
```python
python train.py -net resnet50/densenet201 -gpu
```

### test：
```python
python test.py -net densenet201 -weights checkpoint/densenet201.pth -gpu
```
checkpoint文件见百度网盘  
 
 
## CeiT
CNN_Transformer 文件夹中包含CeiT的相关文件 


### Train :
```
python train.py -c configs/default.yaml --name "name_of_exp"
```

### test :
```python
python test.py -c configs/defaul.yaml --name "test" -p checkpoint/checkpoint.pyt

```
checkpoint 文件见百度网盘
  
  


## Reference:
* [Incorporating Convolution Designs into Visual Transformers](https://arxiv.org/pdf/2103.11816v2.pdf)
* https://github.com/rishikksh20/CeiT-pytorch.git
* https://github.com/weiaicunzai/pytorch-cifar100.git
