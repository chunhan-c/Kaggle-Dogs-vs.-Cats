# Kaggle-Dogs-vs.-Cats

此項目為Kaggle貓與狗的分類競賽, Training dataset一共有25000張的照片(貓跟狗各有125000張), Test dataset共有11000張照片。  
由於此比賽Kaggle已取消了提交功能，為了評估模型的表現，我將Test dataset的前1500張照片手動分類，並使用在Training期間表現最好之pre-trained模型Resnet50(以訓練時間和accuracy作為依據)進行分類。

以下為各pre-trained模型之表現(Training loss, validation loss, accuracy ,平均accuracy(紅色虛線), 所訓練時間):

Alexnet(7 epochs):
![image](https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/alexnet_7_epoch.png)

VGG11(5 epochs):
![image](https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/vgg11_5_epoch.png)

Resnet18(5 epochs):
![image](https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/resnet18_5_epoch.png)


