# Kaggle-Dogs-vs.-Cats

此項目為Kaggle貓與狗的分類競賽, Training dataset一共有25000張的照片(貓跟狗各有125000張), Test dataset共有11000張照片。  
由於此比賽Kaggle已取消了提交功能，為了評估模型的表現，我將Test dataset的前1500張照片手動分類，並使用在Training期間表現最好之pre-trained模型Resnet50(以訓練時間和accuracy作為依據)進行分類。

以下為各pre-trained模型之表現:

Alexnet(7 epochs):
![image]
