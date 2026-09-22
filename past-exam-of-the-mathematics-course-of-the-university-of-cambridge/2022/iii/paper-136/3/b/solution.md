<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\alpha=\sqrt[p]{p}$. The polynomial $X^p-p$ is [Eisenstein](../../../../../../eisenstein-polynomial.md), so $\mathbb Q_p(\alpha)/\mathbb Q_p$ is totally ramified of degree $p$. The cyclotomic extension $\mathbb Q_p(\zeta_p)/\mathbb Q_p$ is totally ramified of degree $p-1$. Their coprime degrees make their intersection trivial, so

$$
K=\mathbb Q_p(\zeta_p,\alpha)
$$

has degree $p(p-1)$ and is totally ramified. It is the splitting field of $X^p-p$, hence Galois.

Normalize $v_K$ by $v_K(K^\times)=\mathbb Z$. Then

$$
v_K(\zeta_p-1)=p,
\qquad v_K(\alpha)=p-1,
$$

so

$$
\varpi=\frac{\zeta_p-1}{\alpha}
$$

is a [uniformizer](../../../../../../uniformizer.md). Write an automorphism as

$$
\sigma_{a,b}(\zeta_p)=\zeta_p^a,
\qquad
\sigma_{a,b}(\alpha)=\zeta_p^b\alpha,
$$

where $a\in\mathbb F_p^\times$ and $b\in\mathbb F_p$. Since

$$
\frac{\sigma_{a,b}(\varpi)}{\varpi}
=\zeta_p^{-b}\frac{\zeta_p^a-1}{\zeta_p-1},
$$

the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) gives valuation one for $\sigma(\varpi)-\varpi$ when $a\ne1$, and valuation $p+1$ when $a=1$, $b\ne0$. Therefore

$$
G_0=G,qquad
G_i=\{\sigma_{1,b}:b\in\mathbb F_p\}\cong\mathbb Z/p\mathbb Z\quad(1\leq i\leq p),
$$

and $G_i=1$ for $i\geq p+1$. These are the [ramification groups of the splitting field of Xp minus p over the p-adic numbers](../../../../../../ramification-groups-of-the-splitting-field-of-xp-minus-p-over-the-p-adic-numbers.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
