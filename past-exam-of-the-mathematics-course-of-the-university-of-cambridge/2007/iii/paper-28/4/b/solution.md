<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\alpha=\sqrt[p]{p}$ and $\lambda=\zeta_p-1$. The polynomial $T^p-p$ is [Eisenstein](../../../../../../eisenstein-criterion.md), so $[\mathbb Q_p(\alpha):\mathbb Q_p]=p$, while the preceding part gives degree $p-1$ for $E$. Both numbers divide $[K:\mathbb Q_p]$ by the [tower law](../../../../../../tower-law.md), and the [compositum](../../../../../../field-compositum.md) degree is at most their product. Coprimality forces $[K:\mathbb Q_p]=p(p-1)$. Since $K$ contains all the roots $\zeta_p^a\alpha$ of $T^p-p$, it is the [splitting field](../../../../../../splitting-field.md) of a [separable polynomial](../../../../../../separable-polynomial.md) and is [Galois](../../../../../../finite-galois-extension.md).

Extend $v_p$ with $v_p(p)=1$. Then $v_p(\alpha)=1/p$, $v_p(\lambda)=1/(p-1)$, and

$$
\boxed{\varpi=\frac{\zeta_p-1}{\sqrt[p]{p}},\qquad v_p(\varpi)=\frac1{p(p-1)}.}
$$

The value group therefore forces the ramification index to be at least $p(p-1)$; it cannot exceed the extension degree. Thus $K/\mathbb Q_p$ is totally ramified and $\varpi$ is a [uniformizer](../../../../../../uniformizer.md) for the normalized valuation $v_K=p(p-1)v_p$.

Write its automorphisms as $\sigma_{a,b}(\alpha)=\zeta_p^a\alpha$ and $\sigma_{a,b}(\zeta_p)=\zeta_p^b$, with $a\in\mathbb F_p$, $b\in\mathbb F_p^\times$. The degree count makes all $p(p-1)$ pairs occur, giving $G\cong\mathbb F_p\rtimes\mathbb F_p^\times$. Their action on the uniformizer is

$$
\frac{\sigma_{a,b}(\varpi)}{\varpi}=\zeta_p^{-a}\frac{\zeta_p^b-1}{\zeta_p-1}.
$$

If $b\ne1$, the residue of this ratio is $b$, so subtracting one gives a unit and $v_K(\sigma_{a,b}(\varpi)-\varpi)=1$. If $b=1$ and $a\ne0$, the ratio is $\zeta_p^{-a}$, giving displacement valuation $1+v_K(\zeta_p^{-a}-1)=p+1$. The identity has infinite displacement valuation.

By the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md), $\sigma\in G_i$ precisely when that displacement valuation is at least $i+1$. Hence the [ramification groups of the splitting field of Xp minus p over the p-adic numbers](../../../../../../ramification-groups-of-the-splitting-field-of-xp-minus-p-over-the-p-adic-numbers.md) have sizes

$$
\boxed{|G_i|=\begin{cases}p(p-1),&i=-1,0,\\p,&1\le i\le p,\\1,&i\ge p+1.\end{cases}}
$$

For $1\le i\le p$ the group itself is $\{\sigma_{a,1}:a\in\mathbb F_p\}\cong C_p$. The lower wild ramification break is $p$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
