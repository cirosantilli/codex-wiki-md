<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [infinite product](../../../../../../infinite-product.md) converges locally uniformly in $\mathbb H$, because $\sum_{n\geq1}|q|^n<\infty$ uniformly on compact subsets. None of its factors vanishes there, and the convergent logarithm of its tail shows that the product is nonzero. Logarithmic differentiation, justified by locally [uniform convergence](../../../../../../uniform-convergence.md), gives

$$
\Theta\log F=1-24\sum_{n\geq1}\frac{nq^n}{1-q^n}
=1-24\sum_{m\geq1}\sigma_1(m)q^m=E_2.
$$

The middle equality groups the absolutely convergent terms $nq^{nr}$ by $m=nr$. Thus $F'/F=2\pi iE_2$.

Let $H(\tau)=\tau^{-12}F(-1/\tau)/F(\tau)$. It is nonzero and [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on the simply connected upper half-plane. Using the printed transformation $E_2(-1/\tau)=\tau^2E_2(\tau)+6\tau/(\pi i)$, its logarithmic [derivative](../../../../../../derivative.md) is

$$
\frac{H'}H=-\frac{12}{\tau}+
\frac{2\pi i}{\tau^2}E_2(-1/\tau)-2\pi iE_2(\tau)=0.
$$

So $H$ is constant. At $\tau=i$ we have $-1/i=i$ and $i^{-12}=1$, giving $H(i)=1$. Therefore $F(-1/\tau)=\tau^{12}F(\tau)$. Also $F(\tau+1)=F(\tau)$ directly from $q=e^{2\pi i\tau}$. Since these two transformations generate $SL_2(\mathbb Z)$, $F$ has the weight-twelve [modular form](../../../../../../modular-form.md) transformation law.

At the unique [modular cusp](../../../../../../cusp-of-a-modular-group.md) its expansion is $F=q+O(q^2)$, so it extends holomorphically with zero value. Hence

$$
\boxed{F\in S_{12}(SL_2(\mathbb Z)),\qquad \Theta F=E_2F.}
$$

This is the [modular discriminant](../../../../../../modular-discriminant.md). The transformed argument contributes $6\tau/(\pi i)$; the converted TeX's numerator $67$ is a transcription error, not the printed relation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
