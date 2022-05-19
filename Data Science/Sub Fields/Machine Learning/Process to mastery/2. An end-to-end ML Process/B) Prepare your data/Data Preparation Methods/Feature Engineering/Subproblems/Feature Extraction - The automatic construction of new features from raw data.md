```ad-warning
Some observations are far too voluminous in their raw state to be modeled by predictive modeling algorithms directly. *Common examples include image, audio, and textual data, but could just as easily include tabular data with millions of attributes.*
```

[Feature extraction](https://en.wikipedia.org/wiki/Feature_extraction) is **a process of automatically reducing the dimensionality of these types of observations into a much smaller set that can be modelled.**

For tabular data, this might include projection methods like Principal Component Analysis and unsupervised clustering methods. For image data, this might include line or edge detection. Depending on the domain, image, video and audio observations lend themselves to many of the same types of DSP methods.

```ad-attention
<mark>Key to feature extraction is that the methods are automatic (although may need to be designed and constructed from simpler methods) and solve the problem of unmanageably high dimensional data, most typically used for analog observations stored in digital formats.
</mark>
```