<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\sigma(z)=\overline z$, componentwise [complex conjugation](../../../../../../complex-conjugation.md). Interpret the printed $|z^2|$ in the potential as $|z|^2=\sum_j|z_j|^2$. With $D=1+|z|^2$, the local [Fubini-Study form](../../../../../../fubini-study-form.md) is

$$
\widetilde\omega_{FS}=\frac{i}{2}\sum_{j,k}
\left(\frac{\delta_{jk}}D-\frac{\overline z_jz_k}{D^2}\right)dz_j\wedge d\overline z_k.
$$

Its [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) under $\sigma$ is

$$
\sigma^*\widetilde\omega_{FS}
=\frac{i}{2}\sum_{j,k}
\left(\frac{\delta_{jk}}D-\frac{z_j\overline z_k}{D^2}\right)d\overline z_j\wedge dz_k
=-\widetilde\omega_{FS},
$$

where the last equality swaps $j,k$ and uses antisymmetry of the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md). Since $\sigma^2=I$, it is an [anti-symplectic involution](../../../../../../anti-symplectic-involution.md), with [fixed-point set](../../../../../../fixed-point-set.md) $\mathbb R^n$. Part (c) gives

$$
\boxed{\mathbb R^n\subset(\mathbb C^n,\widetilde\omega_{FS})\text{ is Lagrangian}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 140](../../../paper-140-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
