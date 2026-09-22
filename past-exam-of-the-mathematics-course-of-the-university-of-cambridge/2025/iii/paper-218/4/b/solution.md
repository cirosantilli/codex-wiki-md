<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Training minimizes the empirical [categorical cross-entropy loss](../../../../../../categorical-cross-entropy-loss.md)

$$
L(\theta)=-\frac1{10000}\sum_{i=1}^{10000}\sum_{k=1}^2y_{ik}\log\widehat p_k(x_i;\theta)
$$

by [stochastic gradient descent](../../../../../../stochastic-gradient-descent.md). The independent validation set monitors generalization, while the small fixed number of epochs limits how long the network can fit training noise; using validation loss for [early stopping](../../../../../../early-stopping.md) would make this safeguard explicit. A forward pass computes all layer activations, class probabilities, and the mini-batch loss. There are $10000/2=5000$ training mini-batches per epoch and hence $5\cdot5000=25000$ training forward passes, in addition to validation evaluation after each epoch.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
