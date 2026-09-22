<h1 id="31j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed sample $z_{1:n}$, its [Empirical Rademacher complexity](../../../../../../empirical-rademacher-complexity.md) is

$$
\boxed{
\widehat{\mathcal R}(\mathcal F(z_{1:n}))
=\mathbb E_\varepsilon\left[
\sup_{f\in\mathcal F}\frac1n\sum_{i=1}^n
\varepsilon_i f(z_i)
\right].
}
$$

Its sample [expected value](../../../../../../expected-value.md) is $\mathcal R_n(\mathcal F)$.

Because every $f\in\mathcal F$ takes values in $\{0,1\}$, replacing one sample point changes $\widehat{\mathcal R}$ by at most $1/n$. Put

$$
s=\sqrt{\frac{\log(3/\delta)}{2n}}.
$$

The lower-tail form of the [Bounded differences inequality](../../../../../../mcdiarmid-s-inequality.md) gives

$$
\mathcal R_n(\mathcal F)
\leq\widehat{\mathcal R}(\mathcal F(Z_{1:n}))+s
$$

outside an event of probability at most $\delta/3$.

For the excess-loss supremum $G$ from part (b), replacing one observation changes $G$ by at most $2/n$. A second application of the same inequality gives

$$
G\leq\mathbb EG+\sqrt{\frac{2\log(3/\delta)}n}
=\mathbb EG+2s
$$

outside another event of probability at most $\delta/3$. On the intersection of these two events, [symmetrization](../../../../../../rademacher-symmetrization-inequality.md) and the [union bound](../../../../../../boole-s-inequality.md) yield

$$
\begin{aligned}
R(\widehat h)-R(h^*)
&\leq G\\
&\leq2\mathcal R_n(\mathcal F)+2s\\
&\leq2\widehat{\mathcal R}(\mathcal F(Z_{1:n}))+4s.
\end{aligned}
$$

This event has [probability](../../../../../../probability-theory-split.md) at least $1-2\delta/3\geq1-\delta$, and $4s=2\sqrt{2\log(3/\delta)/n}$. Thus

$$
\boxed{
R(\widehat h)-R(h^*)
\leq2\widehat{\mathcal R}(\mathcal F(Z_{1:n}))
+2\sqrt{\frac{2\log(3/\delta)}n}.
}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
