<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For binary $A$, conditional covariance satisfies

$$
\operatorname{Cov}(A,Y\mid X)
=\pi(X)\{1-\pi(X)\}
\left\{\mathbb E(Y\mid A=1,X)-\mathbb E(Y\mid A=0,X)\right\}.
$$

By [conditional exchangeability](../../../../../../conditional-exchangeability.md) and [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md), the difference in braces is $\mathbb E[Y(1)-Y(0)\mid X]$. Consequently

$$
\beta
=\mathbb E\!\left[
\pi(X)\{1-\pi(X)\}\{Y(1)-Y(0)\}
\right],
$$

so the required weight is

$$
w(X)=\pi(X)\{1-\pi(X)\}.
$$

This [overlap weight](../../../../../../overlap-weight.md) emphasizes covariate strata with treatment probabilities near one half and downweights strata near a violation of [positivity in causal inference](../../../../../../positivity-assumption.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
