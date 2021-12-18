# Binarization of Deep Embeddings

The objective of any research work is to find methods with very high performance, as simple as possible and, flexible enough that they can be applied to many tasks with little or no modification at all.

With this in mind as a clear objective, we propose a flexible and simple approach to binary representation learning, in which binary codes are generated in an unsupervised way. Additionally, we investigate the network architecture that best suits the hash model to achieve maximum performance, i.e. Siamese and Triplet Networks are used to learn real embeddings of images in continuous-space.

Our method relies on comparisons of the dimensions of real embeddings to obtain binary codes. No threshold function is used, so robustness concerning different tasks is achieved.
As a preprocessing before the binarization step, PCA is performed in the training data to learn a mapping that is used both to reduce the dimension of the real embeddings and to order them in decreasing order according to the variance that each dimension represents. In this way, much more robust binary codes are learned.

The flexibility of the method allows applying it to any task of Object/Scene Recognition with arbitrarily network architecture. 
Experiments are conducted on conventional datasets such as MNIST and CIFAR-10. Moreover, we also evaluate our method in a scene recognition task of a real-word dataset, 'PARTITIONED NORDLAND', so that we can test our model in different and more complex tasks. Our model outperforms the state-of-the-art methods with a much simpler and flexible approach.
