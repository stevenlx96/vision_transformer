# vision_transformer
The study of the differences between the Vision Transformer models(ViT) and Convolutional neural networks(CNNs).


## Overview

1. CNNs are the most popular method used for visual data; however the recent developments of vision transformer models have had comparable or even better results on image classification problems. So the main task of the paper is to answer the question that how a Vit works.
2. In order to answer the question above, the concept of CKA(Centered Kernal Alignment) was widely used.

### CKA(Centered Kernal Alignment)
"A quantitative comparisons of representations within and across networks"
![image](https://user-images.githubusercontent.com/5521243/158394006-ce275df7-f618-4b95-b9da-4b0aa3bcc630.png)



4. One of the most useful parts of Bayesian modeling, the prior, often gets wasted because it is too difficult to calculate them.
5. Deep learning has been used to solve bayesian problems, but success has been limited.
6. In possibly groundbreaking work, the authors show how a kind of self-supervised learning (using artificial generated data) can be used build priors and caclculate posterior probabilities using a Transformer network. 
7. In sample work, this approach outperformed XGBoost and CatBoost, and provided meaningful uncertainty, while training more than 5,000 times faster (from 20 hours to 13 seconds)!
8. More exploration needs to be done to see if the promised holds more generally. 





## Discussion Topic 1

IF the findings in the paper generalize broadly, what impact could this have on future Machine Learning approaches?

## Discussion Topic 2

The approach described fits models 100-5,000 times faster than existing methods. What are some other possible advantages to the approach? What are some possible drawbacks? (HINT: Which is faster to score (or inference)--an XGBoost model or a large(ish) Transformer model)?

## Discussion Topic 3

The models provide excellent uncertainty calibration--they provide not just point estimates, but ranges of uncertainty that are close to true probabilities. How might that be helpful?


## Critical Analysis

In their comparison to machine learning methods (XGBoost and CatBoost), the authors note that they only analyzed datasets from MLBenchmark that were not missing data and that had fewer than 100 predictors, and further simplified the datasets to be balanced. They did not indicate whether their approach was limited to only datasets that met these criteria, or whether this was for expediency. If this is a limitation of the approach, this should have been highlighted. 

 

## Resource links

Original Article: https://arxiv.org/abs/2108.08810
Code designed by community https://github.com/AntixK/PyTorch-Model-Compare

## Code demonstration

The code has not yet been made availalbe.

## Video Recording

Link to video recording.
