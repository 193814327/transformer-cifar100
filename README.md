# cifar100-classification-with-CNN-and-Transformer

本次实验使用CeiT作为 CNN + Transformer 的网络模型，该模型参数量为5.9M
使用 ResNet18 作为CNN对比模型，其模型参数量为11.7M


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
  

## Reference:
* [Incorporating Convolution Designs into Visual Transformers](https://arxiv.org/pdf/2103.11816v2.pdf)
* https://github.com/rishikksh20/CeiT-pytorch.git
* https://github.com/weiaicunzai/pytorch-cifar100.git
