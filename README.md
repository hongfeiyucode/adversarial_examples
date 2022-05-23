# 《AI安全之对抗样本入门》


## 修复

### cannot import name 'zero_gradients'

```Python
#from torch.autograd.gradcheck import zero_gradients

#zero_gradients(img)  
if img.grad is not None :  
    img.grad.zero_()
```


### GPU内存不足，默认为0

```Python
#获取计算设备 默认是CPU
device = torch.device("cuda:1" if torch.cuda.is_available() else "cpu")
```


### show_images_diff前面加上


```Python
%matplotlib inline
```
