**Can we avoid the manual load of prescribing how to construct or extract features from raw data?**

Representation learning or [feature learning](https://en.wikipedia.org/wiki/Feature_learning) is an effort towards this goal.

Modern deep learning methods are achieving some success in this area, such as autoencoders and restricted Boltzmann machines.<mark style="background: #FF5582A6;"> They have been shown to automatically and in a unsupervised or semi-supervised way, learn abstract representations of features (a compressed form), that in turn have supported state-of-the-art results in domains such as speech recognition, image classification, object recognition and other areas.</mark> 

We do not have automatic feature extraction or construction, yet, and we will probably never have automatic feature engineering.

```ad-warning
The abstract representations are prepared automatically, but you cannot understand and leverage what has been learned, other than in a black-box manner. They cannot (yet, or easily) inform you and the process on how to create more similar and different features like those that are doing well, on a given problem or on similar problems in the future. The acquired skill is trapped.
```

Nevertheless, it’s fascinating, exciting and an important and modern part of feature engineering.