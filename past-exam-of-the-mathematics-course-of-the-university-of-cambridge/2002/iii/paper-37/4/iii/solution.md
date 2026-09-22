<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let the annual count be $Y_t=y_t$, with null mean $\lambda_{0t}$ and alternative mean $\theta\lambda_{0t}$. Dividing the two [probability mass functions](../../../../../../probability-mass-function.md) for the [Poisson distributions](../../../../../../poisson-distribution.md) cancels $y_t!$ and the common power of $\lambda_{0t}$:

$$
\frac{f_A(y_t)}{f_0(y_t)}
=e^{-(\theta-1)\lambda_{0t}}\theta^{y_t}.
$$

Consequently the score for the [Poisson likelihood-ratio CUSUM](../../../../../../poisson-likelihood-ratio-cusum.md) is

$$
\boxed{W_t=y_t\log\theta-(\theta-1)\lambda_{0t}.}
$$

At $\theta=2$, this becomes

$$
\boxed{W_t=O\log2-E.}
$$

Under the stated [Poisson](../../../../../../poisson-distribution.md) model this identity is exact, rather than an additional approximation. The approximation in a practical application concerns the mortality model and the use of an estimated expected count.

For $\theta>1$, the expected scores verify the direction of evidence:

$$
\mathbb E_0W_t=\lambda_{0t}[\log\theta-(\theta-1)]<0,
\qquad
\mathbb E_AW_t=\lambda_{0t}[\theta\log\theta-(\theta-1)]>0.
$$

The first inequality follows from $\log\theta<\theta-1$; the second bracket is zero at one and has positive derivative $\log\theta$ above one.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
