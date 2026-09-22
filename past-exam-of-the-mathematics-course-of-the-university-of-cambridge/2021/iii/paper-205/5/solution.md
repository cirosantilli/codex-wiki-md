<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the uncentered [sample covariance matrix](../../../../../sample-covariance-matrix.md)

$$
\widehat\Sigma=\frac1n\sum_{i=1}^nx_ix_i^T,
\qquad
\widehat v_\ell=a_\ell^T\widehat\Sigma a_\ell.
$$

Then $v_\ell=a_\ell^T\Sigma a_\ell$ and, simultaneously for every unit vector $a_\ell$,

$$
|\widehat v_\ell-v_\ell|
\leq\lVert\widehat\Sigma-\Sigma\rVert_{\mathrm{op}}.
$$

Here $\lVert\Sigma\rVert_{\mathrm{op}}=1$ and the [effective rank of a covariance matrix](../../../../../effective-rank-of-a-covariance-matrix.md) satisfies

$$
r(\Sigma)=\operatorname{tr}\Sigma=\sum_{j=1}^d\frac1j\leq1+\log d.
$$

The [Gaussian sample-covariance operator-norm bound](../../../../../gaussian-sample-covariance-operator-norm-bound.md) therefore gives, with probability at least $1-e^{-\delta}$,

$$
\lVert\widehat\Sigma-\Sigma\rVert_{\mathrm{op}}
\leq C_0\left\{
\sqrt{\frac{\log d+1+\delta}{n}}
+\frac{\log d+1+\delta}{n}\right\}.
$$

Under the assumed upper bound on $\log d+1+\delta$, the second term is at most the first. Thus the stronger simultaneous estimate

$$
|\widehat v_\ell-v_\ell|
\leq C_1\sqrt{\frac{\log d+1+\delta}{n}}
$$

holds for every $\ell$. Squaring and using that the displayed ratio is at most one gives the inequality requested in the question after enlarging the universal constant $C$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
