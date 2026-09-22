<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put

$$
\xi_{ik}=\langle X_i,B_k\rangle,
\qquad
\beta_K=\sum_{k=1}^Kc_kB_k,
\qquad
r_i=\langle X_i,\beta-\beta_K\rangle.
$$

With the $n$ by $K$ [design matrix](../../../../../../../design-matrix.md) $\Xi=(\xi_{ik})$, the [scalar-on-function linear model](../../../../../../../scalar-on-function-linear-model.md) becomes

$$
Y=\Xi c+r+\varepsilon.
$$

The [ordinary least squares](../../../../../../../ordinary-least-squares.md) estimator based on the truncated model is

$$
\widehat c=(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}Y
=c+(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}r
+(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}\varepsilon.
$$

Thus the omitted tail produces the conditional bias $(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}r$.

Let

$$
\Sigma_{jk}=\mathbb E[\xi_{1j}\xi_{1k}]
=\langle C_XB_j,B_k\rangle,
\qquad
g_j=\mathbb E[\xi_{1j}r_1]
=\langle C_XB_j,\beta-\beta_K\rangle.
$$

The supplied [weak law of large numbers](../../../../../../../weak-law-of-large-numbers.md) and noise limit give

$$
\widehat c\xrightarrow{p}c+\Sigma^{-1}g.
$$

For a general fixed basis, $g$ need not vanish, so the retained coefficients are asymptotically biased and the estimator is inconsistent even for $c$. Moreover, with fixed $K$ it cannot recover the full slope $\beta$ when $\beta-\beta_K\ne0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 225](../../../../paper-225-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
