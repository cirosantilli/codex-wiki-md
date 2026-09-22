<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N_k(x)$ index the $k$ closest training covariates to $x$. The [K-nearest neighbors algorithm](../../../../../../k-nearest-neighbors-algorithm.md) estimates

$$
\widehat\eta_1(x)=\frac1k\sum_{i\in N_k(x)}Y_i
$$

and predicts one when this average is at least $1/2$.

Small $k$ gives low smoothing bias but high sampling variance and a jagged [decision boundary](../../../../../../decision-boundary.md). Larger $k$ averages more labels, reducing variance and producing a smoother boundary, but it mixes increasingly distant covariates and raises bias. The optimal balance depends on sample size, dimension, and smoothness of $\eta_1$, and is commonly selected by [cross-validation](../../../../../../cross-validation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
