<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the natural [filtration](../../../../../../filtration-probability-theory.md) $\mathcal F_k=\sigma(X_1,\ldots,X_k)$ and define $M_k=S_k-mk$. The increments $X_k-m$ are centered, independent, and square integrable, so their [conditional expectations](../../../../../../conditional-expectation.md) given the past are zero. Thus $(M_k)$ is a [square-integrable](../../../../../../square-integrable-function.md) [martingale](../../../../../../martingale-split.md) with $M_0=0$. [Independence](../../../../../../independent-random-variables.md) gives

$$
\mathbb E|M_n|^2=\operatorname{Var}\!\left(\sum_{j=1}^n(X_j-m)\right)=n\sigma^2.
$$

Applying the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) yields

$$
\boxed{\mathbb E\!\left[\max_{0\leq k\leq n}|S_k-mk|^2\right]\leq4n\sigma^2.}
$$

This includes $\sigma^2=0$, when every centered increment vanishes [almost surely](../../../../../../almost-sure-convergence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
