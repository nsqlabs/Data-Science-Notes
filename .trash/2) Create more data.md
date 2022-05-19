Deep learning algorithms often perform better with more data.

We mentioned this in the last section.

If you can’t reasonably get more data, you can invent more data.

-   If your data are vectors of numbers, create randomly modified versions of existing vectors.
-   If your data are images, create randomly modified versions of existing images.
-   If your data are text, you get the idea…

Often this is called [data augmentation](https://machinelearningmastery.com/how-to-configure-image-data-augmentation-when-training-deep-learning-neural-networks/) or data generation.

You can use a generative model. You can also use simple tricks.

For example, with photograph image data, you can get big gains by randomly shifting and rotating existing images. It improves the generalization of the model to such transforms in the data if they are to be expected in new data.

This is also related to adding noise, what we used to call adding jitter. It can act like a regularization method to curb overfitting the training dataset.