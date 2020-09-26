# Kaggle-Dogs-vs.-Cats

此項目為Kaggle貓與狗的分類競賽, Training dataset一共有25000張的照片(貓跟狗各有12500張), Test dataset共有11000張照片。
這個github中以Google Colab的 GPU 進行操作，並展現了各種pre-trained模型的實驗結果(Alexnet, VGG11, Resnet18, Resnet50, Resnet152)。
從下列圖片可以看出，Resnet表現得最好，若將Resnet50與152比，Resnet152表現得更好，accuracy約高0.01。
但是因為Resnet152的深度更深，在使用GPU下，所需要的訓練時間為33.39分鐘，相較於Resnet50的27.79分鐘，所需時間更長。  

<div align=center><img src="https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/resnet50_v.s_resnet152.png" alt="Resnet50 v.s. Resnet152"/></div> 



由於此比賽Kaggle已取消了提交功能，為了評估模型的表現，我將Test dataset的前1500張照片手動分類，並使用在Training期間表現最好之pre-trained模型Resnet152(以訓練時間和accuracy作為依據)進行分類，得到 0.9813 accuracy。



以下為所有pre-trained 模型中表現前二名，Resnet50 以及 Resnet152:

Resnet50(5 epochs):  
<div align=center><img src="https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/resnet50_5e.png"/></div> 


Resnet152(5 epochs):  
<div align=center><img src="https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/resnet152_5e.png"/></div>  





以下為其他pre-trained模型之表現(Training loss, validation loss, accuracy ,平均accuracy(紅色虛線), 所訓練時間):

Alexnet(7 epochs):
![image](https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/alexnet_7_epoch.png)


VGG11(5 epochs):
![image](https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/vgg11_5_epoch.png)

Resnet18(5 epochs):
![image](https://github.com/chunhan-c/Kaggle-Dogs-vs.-Cats/blob/master/resnet18_5_epoch.png)


