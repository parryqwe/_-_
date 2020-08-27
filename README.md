# 手寫辨識分類
## 資料介紹(來源:http://yann.lecun.com/exdb/mnist/ )
### 訓練集資料:60000筆
### 測試集資料:10000筆
### 特徵維度:784維
### 類別數:10類
## 模型
### 線性隱藏層1:隱含維度500，初始權重normal(0,0.02)，初始偏差normal(0,0.01)
### relu函數
### 線性隱藏層2:隱含維度250，初始權重normal(0,0.02)，初始偏差normal(0,0.01)
### relu函數
### 輸出層:維度10，初始權重normal(0,0.02)，初始偏差normal(0,0.01)
### 損失函數:$CE = -(1/N)\sum_{i=1}^{N}y_ilog(\hat{y}_i) + (1-y_i)log(1-\hat{y}_i)$

### 更新梯度:momentum(momentum=0.9,learning_rate=0.01)
### 預測結果:softmax函數
