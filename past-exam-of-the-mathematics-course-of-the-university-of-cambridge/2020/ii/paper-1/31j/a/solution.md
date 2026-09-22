<h1 id="31j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\varepsilon_1,\ldots,\varepsilon_n$ be [independent](../../../../../../independent-random-variables.md) [Rademacher signs](../../../../../../rademacher-distribution.md), also independent of the [i.i.d. sample](../../../../../../independent-and-identically-distributed-random-variables.md) $Z_{1:n}$. With the $1/n$ normalization, the [Rademacher complexity](../../../../../../rademacher-complexity.md) is

$$
\mathcal R_n(\mathcal F)
=\mathbb E_{Z,\varepsilon}\left[
\sup_{f\in\mathcal F}\frac1n\sum_{i=1}^n
\varepsilon_i f(Z_i)
\right].
$$

The [Rademacher symmetrization inequality](../../../../../../rademacher-symmetrization-inequality.md) is

$$
\boxed{
\mathbb E\left[
\sup_{f\in\mathcal F}\frac1n\sum_{i=1}^n
\bigl(f(Z_i)-\mathbb Ef(Z_i)\bigr)
\right]
\leq2\mathcal R_n(\mathcal F).
}
$$

The [Bounded differences inequality](../../../../../../mcdiarmid-s-inequality.md) states that if $W=g(U_1,\ldots,U_n)$ for [independent random variables](../../../../../../independent-random-variables.md) $U_i$, and replacing only $U_i$ can change $g$ by at most $c_i$, then for every $t>0$,

$$
\boxed{
\mathbb P(W-\mathbb EW\geq t)
\leq\exp\left(-\frac{2t^2}{\sum_{i=1}^nc_i^2}\right).
}
$$

The same estimate holds for the lower tail $\mathbb P(W-\mathbb EW\leq-t)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31J](../../31j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
