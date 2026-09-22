<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For one-hot labels $y_{il}$ and predicted probabilities $p_{il}(\theta)$, the [categorical cross-entropy loss](../../../../../../categorical-cross-entropy-loss.md) is

$$
L(\theta)=-\sum_{i=1}^n\sum_{l=1}^{26}y_{il}\log p_{il}(\theta).
$$

Stochastic gradient descent initializes $\theta$, randomly orders the observations in each of five epochs, and for each single-observation batch computes a forward pass, the sample loss, and its gradient, then updates

$$
\theta\leftarrow\theta-\eta\nabla_\theta L_i(\theta).
$$

[Backpropagation](../../../../../../backpropagation.md) is used after the forward loss evaluation to compute this gradient from the output layer back through the hidden layers.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
