---
layout: posts
---

One can think of deep learning on images as a series of transformations on data volumes where the data volumes represent image features and the network represents transform functions from one volume to another. Through the process of training the network and tuning the parameters, we are making an effort to streamline this transformation towards a performance objective. In the case of the image classification, that would be to reduce misclassification or classification error. The volumes would represent intermediate representations of objects, from pixels to blobs to abstract objects to objects to their semantic description. The last volume is the semantic description which is just an array of probabilities for each classification category.