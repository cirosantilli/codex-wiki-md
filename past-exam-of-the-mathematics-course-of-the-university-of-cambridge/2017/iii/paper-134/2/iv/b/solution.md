<h1 id="2/iv/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $C\in\operatorname{Neg}(K_X)$. The [arithmetic adjunction formula on a smooth surface](../../../../../../../arithmetic-adjunction-formula-on-a-smooth-surface.md) gives

$$
2p_a(C)-2=C^2+K_X\cdot C,\qquad p_a(C)\ge0.
$$

We first exclude $C^2\ge0$, following the PDF's hint and the finiteness proved in (a).

If $C^2=0$, adjunction and $K_X\cdot C<0$ force $p_a(C)=0$ and $K_X\cdot C=-2$. An integral projective curve of [arithmetic genus](../../../../../../../arithmetic-genus.md) zero is a [smooth rational curve](../../../../../../../smooth-rational-curve.md): normalization and the nonnegative singularity-length correction show both normalization genus and singularity correction vanish. Part (iii) makes $C$ [semiample](../../../../../../../semiample-divisor.md). Choose a basepoint-free $|mC|$. Over the infinite algebraically closed [field](../../../../../../../field.md), a general section avoids containing any of the finitely many curves of $\operatorname{Neg}(K_X)$ as a component. Its effective divisor $G$ then has $K_X\cdot G\ge0$, but $K_X\cdot G=mK_X\cdot C<0$, a contradiction.

If $C^2>0$, [Riemann–Roch theorem for algebraic surfaces](../../../../../../../riemann-roch-theorem-for-algebraic-surfaces.md) and [Serre duality](../../../../../../../serre-duality.md) show $h^0(X,mC)$ is unbounded. Indeed $h^2(X,mC)=h^0(X,K_X-mC)=0$ for $m\gg0$, because the latter divisor has negative intersection with a fixed [ample](../../../../../../../ample-line-bundle.md) divisor. Hence

$$
h^0(X,mC)\ge\chi(X,\mathcal O_X)+\tfrac12(m^2C^2-mK_X\cdot C)\longrightarrow\infty.
$$

There is therefore some $m$ with $h^0(X,mC)>h^0(X,(m-1)C)$, giving a section whose divisor does not contain $C$. The canonical section of $mC$ does not vanish identically along any other curve. A general linear combination of these two sections consequently contains none of the finite set $\operatorname{Neg}(K_X)$, again contradicting its negative canonical intersection. Thus $C^2<0$.

Now put $a=-C^2\ge1$ and $b=-K_X\cdot C\ge1$. Adjunction gives

$$
-a-b=2p_a(C)-2\ge-2.
$$

It follows that $a=b=1$ and $p_a(C)=0$. Hence

$$
\boxed{C\cong\mathbb P^1,\qquad C^2=-1,\qquad K_X\cdot C=-1.}
$$

The general-section argument only avoids finitely many proper linear subspaces, so it works over any algebraically closed field, including positive characteristic.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iv](../../iv.md)
3. [2](../../../2.md)
4. [Paper 134](../../../../paper-134-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
