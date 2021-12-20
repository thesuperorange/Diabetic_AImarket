# Diabetic_AImarket


## Introduction

* 目標：透過有標記之眼底影像來偵測是否有糖尿病引發的視網膜病變
* 類別：分為五種嚴重程度
    - 0 - No DR
    - 1 - Mild
    - 2 - Moderate
    - 3 - Severe
    - 4 - Proliferative DR
* framework: Pytorch

## Data preparation
* download
  [data.zip](https://superorange.cos.twcc.ai/AI-market_Diabetic_retinopathy_detection/data.zip)

* For training
    * Text data
        * train_img.csv / train_img_small.csv
        * train_label.csv/ train_label_small.csv
        * test_img.csv/ test_img_small.csv
        * test_label.csv/ test_label_small.csv
    * Image data
        * data/<#>_left.jpeg
        * data/<#>_right.jpeg


## 資料展示

- [1.fundus_data.ipynb](https://github.com/thesuperorange/Diabetic_AImarket/blob/main/1.fundus_data.ipynb)

* 內容--資料觀察
    1. label distribution
        ![](image/label_distribution.png)

    2. preview images

        ![](image/preview_images.png)



## 訓練模型
- [2.DR_main.ipynb](https://github.com/thesuperorange/Diabetic_AImarket/blob/main/2.DR_main.ipynb)

* 內容
    1. Dataloader
    2. Training 
    3. Plot results

        * accuracy comparison

            ![](image/accuracy_compare.png)

        * confusion matrix

            ![](image/confusion_matrix.png)


## 模型佈署
- [3.deploy_model.ipynb](https://github.com/thesuperorange/Diabetic_AImarket/blob/main/3.deploy_model.ipynb)


## Reference
* From Kaggle:
    https://www.kaggle.com/c/diabetic-retinopathy-detection#description
