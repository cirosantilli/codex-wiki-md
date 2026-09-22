<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $\Theta=(2\pi i)^{-1}d/d\tau$. For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, differentiating the weight-$k$ law gives

$$
(\Theta f)(\gamma\tau)
=(c\tau+d)^{k+2}\Theta f(\tau)
+\frac{kc}{2\pi i}(c\tau+d)^{k+1}f(\tau).
$$

The transformations of $E_2$ under the generators $S,T$, and the chain rule for their compositions, give

$$
E_2(\gamma\tau)=(c\tau+d)^2E_2(\tau)+\frac{12c}{2\pi i}(c\tau+d).
$$

Equivalently, one can check just $S,T$ in the next cancellation, since they generate the group. Substituting these formulas into

$$
D_kf=\Theta f-\frac{k}{12}E_2f
$$

cancels the extra term and gives $(D_kf)(\gamma\tau)=(c\tau+d)^{k+2}D_kf(\tau)$. Both constituents are [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on $\mathbb H$ and have [Fourier expansions of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md) with nonnegative exponents, so $D_kf$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) at the [modular cusp](../../../../../../cusp-of-a-modular-group.md). Thus

$$
\boxed{D_k:M_k\longrightarrow M_{k+2}.}
$$

This operator is the [Serre derivative](../../../../../../serre-derivative.md).

If $f=\sum_{n\geq0}a_nq^n$, then its [derivative](../../../../../../derivative.md) has constant coefficient zero, while $E_2$ has constant coefficient one. Therefore

$$
a_0(D_kf)=-\frac{k}{12}a_0(f).
$$

For $k\ne0$ this vanishes exactly when $a_0(f)=0$, proving the claimed [cusp form](../../../../../../cusp-form.md) equivalence in the intended positive-weight setting. At **weight zero the printed equivalence is false**: $f=1$ is a noncuspidal weight-zero [modular form](../../../../../../modular-form.md), but $D_0f=0$ belongs to $S_2$. Indeed all weight-zero forms are constants by [compactness](../../../../../../compact-space.md) of $X(1)$. Negative-weight level-one [modular forms](../../../../../../modular-form.md) are zero by the [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md), so there is no further nonzero exception. The transformation and holomorphy conclusion for $D_kf$ remains true at weight zero.

## ↑ Ancestors (11)

1. [B](../b.md)
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
