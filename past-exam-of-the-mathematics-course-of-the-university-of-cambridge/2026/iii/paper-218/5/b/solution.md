<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Stochastic gradient descent](../../../../../../stochastic-gradient-descent.md) replaces the full empirical-loss gradient by the gradient on a randomly ordered observation or mini-batch, then updates $\theta\leftarrow\theta-\eta\widehat\nabla L(\theta)$. The training half contains $768/2=384$ observations, so batches of 16 give $384/16=24$ updates per epoch. Over 100 epochs every parameter is updated $2400$ times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
