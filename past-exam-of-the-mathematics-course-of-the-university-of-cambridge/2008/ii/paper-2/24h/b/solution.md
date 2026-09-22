<h1 id="24h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The planar [planar isoperimetric inequality](../../../../../../planar-isoperimetric-inequality.md) is $4\pi|\Omega|\le|\partial\Omega|^2$, with equality exactly for a disk. For one boundary component of length $L$, take its unit-speed periodic parametrization $\gamma=(x,y)$ and subtract its mean position. Green's area formula and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
|A_{\rm signed}|=\frac12\left|\int_0^L(xy'-yx')ds\right|\le\frac12\left(\int_0^L|\gamma|^2ds\right)^{1/2}\left(\int_0^L|\gamma'|^2ds\right)^{1/2}.
$$

Apply the periodic [Wirtinger inequality](../../../../../../wirtinger-inequality.md) to each mean-zero coordinate: $\int|\gamma|^2\le(L/2\pi)^2\int|\gamma'|^2$. Since unit speed gives the final integral $L$, it follows that $|A_{\rm signed}|\le L^2/(4\pi)$. For several boundary components, orient each with the domain on its left. Green's formula, followed by the [triangle inequality](../../../../../../triangle-inequality.md), gives

$$
|\Omega|\le\frac1{4\pi}\sum_jL_j^2\le\frac1{4\pi}\left(\sum_jL_j\right)^2.
$$

This proves the stated inequality, including disconnected domains or holes. Equality permits only one component; equality in the two integral inequalities makes its coordinates first sine-cosine harmonics with the corresponding orthogonal rotation relation. Unit speed then makes the curve a circle, so its domain is a disk. Conversely disks attain equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24H](../../24h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
