# vision_transformer
The study of the differences between the Vision Transformer models(ViT) and Convolutional neural networks(CNNs).


## Overview

1. CNNs are the most popular method used for visual data; however the recent developments of vision transformer models have had comparable or even better results on image classification problems. So the main task of the paper is to answer the question that how a ViT works.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/conv.png?raw=true)

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/attetion.png?raw=true)

2. In order to answer the question above, the first concept we will use is called CKA(Centered Kernal Alignment).

### CKA(Centered Kernal Alignment)
"A quantitative comparisons of representations within and across networks"

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/cka%20formula.png?raw=true)

where
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/x.png?raw=true) and 
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/y.png?raw=true), 
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/k.png?raw=true) and
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/l.png?raw=true) respectively.

HSIC stands for the Hilbert-Schmidt independence criterion
Where we have
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/h.png?raw=true),
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/kp.png?raw=true), 
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/lp.png?raw=true), and
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/kl.png?raw=true)

3. Applying the CKA concept within networks, we could see ViTs having highly similar representations throughout the model, while the ResNet models show much lower similarity between lower and higher layers.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/layers%20inside.png?raw=true)


4. Applying the CKA concept across networks, we could see ViTs and ResNet models have similar representations at the very beginning of the model, where the size of that portion from ViTs is much smaller

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/layers%20across.png?raw=true)

5. After the study of the structures within and across networks, the paper studies the local& global representations next using the concept of attention distance.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/attention%20head.png?raw=true)

6. The scaling of dataset also affects the model performance, and its telling us the importance of the local features.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/local%20attention.png?raw=true)

7. Combining the attention distance and CKA, we can study the similarities between the ViT and CNNs.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/combin.png?raw=true)

8. The skip connections also play a more significant role in ViT rather than in CNNs.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/skip.png?raw=true)

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/skiplayer.png?raw=true)

9. Higher layers of ViT maintain spatial location information more faithfully than ResNets.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/spatial.png?raw=true)

10. Finally we study the effect of scaling the datasize and model size.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/datasize.png?raw=true)
![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/modelsize.png?raw=true)

## Discussion Topic 1

After finding the similiarities and differences here, how could we apply them?

## Discussion Topic 2

Since the performance of ViT here is generally beating CNN models, can it fully replace the role of CNN? Or is there any condition that CNN is more prefered?

## Discussion Topic 3

We saw how self attention mechanics can work both in language processing areas and visual classification areas. What else can they apply to?


## Critical Analysis

First, the format of the paper is confusing. The figures and the texts are not combining together.

![image](https://github.com/stevenlx96/vision_transformer/blob/main/images/paper.png?raw=true)

Also the authors didn't show their original code as well as the dataset they are using, so it is quite hard for readers to fully go through their methods. Moreover, just like the author addressed in their drawbacks, that this whole paper is based on the concept of CKA. It might be better for further study by using a different metriks to determine the similaritis and differences between the two models.5

## Resource links

Original Article: https://arxiv.org/abs/2108.08810

Code designed by community https://github.com/AntixK/PyTorch-Model-Compare

## Code demonstration

The code has not yet been made availalbe.

## Video Recording

Link to video recording.
