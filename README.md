# Emotion-Detection-Model
## 資料預處理：(*2grayface.ipynb*) 
載入OpenCV，並使用OpenCV中已經訓練過的人臉辨識模型文件*haarcascade_frontalface_default.xml* 來協助處理圖片  
進行灰階以及裁減到相同大小，最後再重新命名。

###### 原始資料
![image](https://user-images.githubusercontent.com/30427256/110300140-8058fb00-8031-11eb-81b5-cf432af70232.png '原始資料')

###### 處理過後
![image](https://user-images.githubusercontent.com/30427256/110302045-c57e2c80-8033-11eb-8ab8-6b32904473b5.png '處理過後')

處理過後的資料分配到train valid test三個資料夾內，裡面各自再細分成7類情緒

![image](https://user-images.githubusercontent.com/30427256/110303798-c9ab4980-8035-11eb-876d-88270a698050.png)
![image](https://user-images.githubusercontent.com/30427256/110304585-bba9f880-8036-11eb-9081-724c04be7ec2.png)

## 模型訓練：(*emotion_detect.ipynb*)  
建立CNN模型並使用資料進行訓練，測試不同的參數來提高準確度
