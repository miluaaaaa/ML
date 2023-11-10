# 利用ResNet网络图像分类报告

-数据集

-主要工作

-问题和总结

## 数据集

本任务提供了一个花数据集

https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz

其中的有五种花，daisy,dandelion,roses,sunflowers,tulips

flower_data中含有train:val=9:1

## 主要工作

### 网络

利用resnet34,resnet50,resnet101,resnext50_32x4d,resnext101_32x8d网络进行对比实验

### 策略

优化器：Adam

每次输入照片批量：16

epochs：150

计算误差的算法:cross entropy loss(交叉熵损失)

#### ResNet34

![image-20231110145759029](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110145759029.png)

![image-20231110145949699](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110145949699.png)

#### ResNet50

![image-20231110150056517](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110150056517.png)

![image-20231110150143261](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110150143261.png)

#### ResNet101

![image-20231108190153418](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231108190153418.png)

![image-20231108190207025](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231108190207025.png)

### Resnext50_32x4d

![image-20231110150239735](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110150239735.png)

![image-20231110150311518](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110150311518.png)

### Resnext101_32x8d

![image-20231110150404065](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110150404065.png)

![image-20231110150444730](C:\Users\10476\AppData\Roaming\Typora\typora-user-images\image-20231110150444730.png)

## 问题总结

吐槽：我实在找不到这些网络得到结果后的差异，可能是我方法不对