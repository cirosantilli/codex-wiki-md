<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\widehat G$ be the group of all [Dirichlet characters](../../../../../../dirichlet-character.md) modulo $q$, where $G=(\mathbb Z/q\mathbb Z)^\times$, and consider

$$
F(s)=\prod_{\chi\in\widehat G}L(s,\chi).
$$

For $p\nmid q$, let $f_p$ be the order of $p$ in $G$. The values $\chi(p)$ run through the $f_p$th roots of unity, each $|G|/f_p$ times, so the local factor is

$$
\prod_{\chi\in\widehat G}(1-\chi(p)p^{-s})^{-1}
=(1-p^{-f_ps})^{-|G|/f_p}.
$$

For $p\mid q$ the local factor is one. Thus the [Dirichlet series](../../../../../../dirichlet-series.md) for $F$ has nonnegative coefficients.

The principal-character factor has a simple pole at $s=1$, while every nonprincipal [Dirichlet L-function](../../../../../../dirichlet-l-function.md) is entire. If some nonprincipal $L(1,\chi)$ vanished, its zero would cancel that pole and make $F$ entire. The [Landau theorem for a Dirichlet series with nonnegative coefficients](../../../../../../landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients.md) would then force the Dirichlet series of $F$ to converge for every real $s$. This is impossible: its coefficient at $m^{|G|}$ is at least one for every $m$ coprime to $q$, as is clear from the local factors. Hence

$$
\boxed{L(1,\chi)\ne0\qquad
\text{for every nonprincipal }\chi.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
