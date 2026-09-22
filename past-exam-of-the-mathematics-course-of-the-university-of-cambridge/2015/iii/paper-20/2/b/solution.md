<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compute each [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md) by tensoring with the [residue field](../../../../../../residue-field.md) of the chosen base point.

For the first map, put $L=\kappa(\mathfrak p)$ for a point $\mathfrak p$ of $\operatorname{Spec}k[T]$ and let $t$ be the image of $T$ in $L$. Then

$$
\boxed{X_{\mathfrak p}=\operatorname{Spec}L[U]/(U^2-t^2).}
$$

If the [characteristic of a field](../../../../../../characteristic-of-a-field.md) is not two and $t\ne0$, the two factors $U-t$ and $U+t$ are coprime, so the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives $L[U]/(U^2-t^2)\simeq L\times L$: the [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md) is two distinct $L$-points. If $t=0$, its ring is $L[U]/(U^2)$, a [dual number](../../../../../../dual-number.md) ring, so it is a [nonreduced double point](../../../../../../nonreduced-double-point.md). In characteristic two, $U^2-t^2=(U-t)^2$ at every point, giving a [nonreduced double point](../../../../../../nonreduced-double-point.md) in every [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md). This covers the [generic point](../../../../../../generic-point.md), where $L=k(T)$, as well as [closed points](../../../../../../closed-point.md) defined by irreducible polynomials.

For the arithmetic map, the generic [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md) is

$$
\boxed{\operatorname{Spec}\mathbb Q[T]/(T^2+1)=\operatorname{Spec}\mathbb Q(i).}
$$

Over a [closed point](../../../../../../closed-point.md) $(p)$ it is $\operatorname{Spec}\mathbb F_p[T]/(T^2+1)$. At $p=2$ this is $\operatorname{Spec}\mathbb F_2[\epsilon]/(\epsilon^2)$, since $T^2+1=(T+1)^2$. For odd $p$, the [finite field](../../../../../../finite-field.md) multiplicative group is cyclic, and $-1$ is a square exactly when $p\equiv1\pmod4$. Thus

$$
\boxed{X_{(p)}\simeq
\begin{cases}
\operatorname{Spec}(\mathbb F_p\times\mathbb F_p),&p\equiv1\pmod4,\\
\operatorname{Spec}\mathbb F_{p^2},&p\equiv3\pmod4,\\
\operatorname{Spec}\mathbb F_2[\epsilon]/(\epsilon^2),&p=2.
\end{cases}}
$$

In the second case there is one degree-two [closed point](../../../../../../closed-point.md) over $\mathbb F_p$, which becomes two points after extending the [residue field](../../../../../../residue-field.md) to an algebraic closure. The case $p=2$ remains nonreduced after such extension.

For $\operatorname{Spec}\mathbb C\to\operatorname{Spec}\mathbb Z$, the unique source point maps to the [generic point](../../../../../../generic-point.md) $(0)$. Since all nonzero integers are invertible in $\mathbb C$,

$$
\boxed{X_{(0)}=\operatorname{Spec}\mathbb C,\qquad X_{(p)}=\varnothing\text{ for every prime }p.}
$$

Indeed $\mathbb C\otimes_{\mathbb Z}\mathbb Q=\mathbb C$, whereas $\mathbb C\otimes_{\mathbb Z}\mathbb F_p=\mathbb C/p\mathbb C=0$. The distinction between a reduced split [scheme-theoretic fibre](../../../../../../scheme-theoretic-fibre.md) and a [nonreduced double point](../../../../../../nonreduced-double-point.md) is essential in the first two examples.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
