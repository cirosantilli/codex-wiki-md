<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose $\beta$ with $\beta^{p(p-1)}=-p$ and put $N=p(p-1)$. The [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) $T^N+p$ shows that $L=\mathbb Q_p(\beta)$ has degree $N$, is [totally ramified](../../../../../../totally-ramified-extension.md), and has [uniformizer](../../../../../../uniformizer.md) $\beta$. Its subfield $\mathbb Q_p(\beta^p)$ is the field $K$ from the previous part. Because $p$ is odd,

$$
a=-\beta^{p-1}\quad\text{satisfies}\quad a^p=p.
$$

Thus $L$ contains $a$ and $\zeta_p$, and contains all roots $a\zeta_p^j$ of $T^p-p$. Conversely $[\mathbb Q_p(a):\mathbb Q_p]=p$, while $[K:\mathbb Q_p]=p-1$. Their coprime degrees force their compositum to have degree $N$. It is contained in $L$ and hence equals it. Therefore **$L$ is exactly the splitting field**, not merely an extension containing it.

The [Galois group](../../../../../../galois-group.md) has a normal subgroup $H=\operatorname{Gal}(L/K)$ of order $p$, acting by $\beta\mapsto\zeta_p^j\beta$. The $(p-1)$st [roots of unity](../../../../../../root-of-unity.md) already lie in $\mathbb Q_p$ by the [Hensel lemma](../../../../../../hensel-s-lemma.md). The maps $\beta\mapsto\omega\beta$, with $\omega^{p-1}=1$, supply a complement of order $p-1$. Its conjugation acts faithfully on $H$, so $G\cong C_p\rtimes\mathbb F_p^\times$.

Normalize $v_L(\beta)=1$. Total ramification and the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) reduce the calculation to $i_G(\sigma)=v_L(\sigma\beta-\beta)$. For nonidentity $\sigma\in H$,

$$
i_G(\sigma)=1+v_L(\zeta_p^j-1)=1+p,
$$

since $e(L/K)=p$ and $v_K(\zeta_p^j-1)=1$. For $\sigma\notin H$, write $\sigma\beta=\omega\zeta_p^j\beta$ with $\omega\ne1$. Its multiplier has residue $\overline\omega\ne1$, so $i_G(\sigma)=1$. The [lower ramification numbering](../../../../../../lower-ramification-numbering.md) is therefore

$$
\boxed{G_{-1}=G_0=G,\qquad G_1=\cdots=G_p=H\cong C_p,\qquad G_{p+1}=1.}
$$

All later groups are trivial. The wild lower break is $p$, not one. In the [upper ramification numbering](../../../../../../upper-ramification-numbering.md), the [Herbrand function](../../../../../../herbrand-function.md) sends this break to $p/(p-1)$: $G^0=G$, $G^u=H$ for $0<u\leq p/(p-1)$, and $G^u=1$ above it.

As an independent consistency check, the [different exponent from ramification groups](../../../../../../different-exponent-from-ramification-groups.md) is $(N-1)+p(p-1)=2N-1$. The derivative of the [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) gives the same answer, $v_L(N\beta^{N-1})=N+(N-1)$, since $v_L(p)=N$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
