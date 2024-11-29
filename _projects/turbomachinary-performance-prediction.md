---
layout: post
title: Turbo Performance Prediction
description: Predicting the Performance of Compressor/Blower Systems using AI
image: "/assets/images/mlpArch.png"
---


Predicting the Performance of Compressor/Blower Systems using AI
============

Introduction:
Performance maps are a popular tool for analyzing and predicting the operating characteristics of a turbine, such as efficiency, pressure ratio, and flow rate. They are critical to system evaluation because they provide insight into how a turbine performs under different operating conditions. By visually representing performance metrics through performance maps, users can identify the optimal operating range and run blowers accordingly in industrial applications. When blower performance maps rely solely on real-world data, they are often inefficient due to the limited number of data points, which prevents accurate comparisons and predictions. Therefore, it is common to use linear interpolation or curve fitting to make the data a little denser based on the acquired data. In this project, we created and presented three model to predict performance and compared the results with predictions using a linear regression curve. 


Proposed Model Architecture
------------

![MLP Only](https://soysilver.github.io/soysilvery/assets/images/Architecture.png)
![MLP + Self Attention](https://soysilver.github.io/soysilvery/assets/images/mlpAttention.png)




Results
------------

|          | Polynomial Fitting |MLP| CNN + MLP |MLP + Self Attention|
|:--------:|:-------:|:-------:|:--------:|:-------:|
|    MAE   | 75.1555 | 11.7533 | 11.6837 | 11.6079 |
| Flow Rate MAE | 10.506 |3.8732 | 3.7618 | 3.7711 |
| Power MAE | 139.805 | 19.6333 | 19.6055 | 19.4446|
| Flow Rate (%)| 93.9665 | 97.8463 | 97.9082 |97.9030 |
| Power (%)| 96.8410 | 99.5472 | 99.5479 | 99.5516 |

Experiments showed that the proposed models outperformed the traditional polynomial method. 
In addition, the models that reflect the relationships within a piece of data were more effective in training.


Publications
------------

Korea Patent (). Under Review.(will be added at 12/3, 2024)

[Yun-sok Ha, Jongyoung Kim, Soyeon Lee, and Yong-Bok Lee, “Research on Optimal Operation of Compressor utilizing Multi-Layer Perceptron and Polynomial Curve Fitting”, Korean Society for Fluid Machinery (Jul, 2024)](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11935183)
[Soyeon Lee, Yun-sok Ha,Jongyoung Kim, and Yong-Bok Lee, “Predicting the Performance of Blower Systems using Multi-Layer-Perceptron(MLP) Architecture with Real Data”, Korean Society for Fluid Machinery (Dec, 2024)]() (will be added at 12/6, 2024)