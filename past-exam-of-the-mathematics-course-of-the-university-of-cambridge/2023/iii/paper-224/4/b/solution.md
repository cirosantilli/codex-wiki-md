<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
S_n=\sum_{i=1}^nX_i^{(n)}.
$$

Here $S_n$ has the [binomial distribution](../../../../../../binomial-distribution.md) with parameters $(n,\lambda/n)$. Part a, now with independent coordinates, gives

$$
D_e(P_{S_n}\Vert\operatorname{Poisson}(\lambda))
\leq n(\lambda/n)^2=\frac{\lambda^2}{n}.
$$

By [Pinsker's inequality](../../../../../../pinsker-s-inequality.md), the probability mass functions therefore converge in total variation, and in particular $S_n$ [converges in distribution](../../../../../../convergence-in-distribution.md) to $Z\sim\operatorname{Poisson}(\lambda)$.

The joint probability of the observed row depends only on $S_n$:

$$
P_n(X_1^{(n)},\ldots,X_n^{(n)})
=\left(\frac\lambda n\right)^{S_n}
\left(1-\frac\lambda n\right)^{n-S_n}.
$$

Taking logarithms in any fixed base and choosing $c_n=\log n$ gives

$$
-\frac1{c_n}\log P_n(X_1^{(n)},\ldots,X_n^{(n)})
=a_nS_n+b_n,
$$

where

$$
a_n=\frac{\log(n/\lambda)+\log(1-\lambda/n)}{\log n}\longrightarrow1,
\qquad
b_n=-\frac{n\log(1-\lambda/n)}{\log n}\longrightarrow0.
$$

The convergence lemma supplied in the question now yields

$$
-\frac1{\log n}\log P_n(X_1^{(n)},\ldots,X_n^{(n)})
\xrightarrow{d}Z,
\qquad Z\sim\operatorname{Poisson}(\lambda).
$$

This sparse triangular array therefore has a random limiting normalized self-information rather than the constant limit in the usual [asymptotic equipartition property](../../../../../../asymptotic-equipartition-property.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
