<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The conclusion holds in dimension two.** Shift and change sign to obtain a nonnegative [harmonic function](../../../../../../harmonic-function.md) $v$. Its circular mean satisfies

$$
m(r)=\frac1{2\pi}\int_0^{2\pi}v(r\cos\theta,r\sin\theta)\,d\theta,\qquad
m''+r^{-1}m'=0.
$$

Here the angular second derivative in the polar-coordinate [Laplacian](../../../../../../laplacian.md) integrates to zero. Thus $m(r)=a\log r+b$; nonnegativity for every $r>0$ forces $a=0$. For $|x|=r$, the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) and nonnegativity give

$$
v(x)\leq\frac4{\pi r^2}\int_{r/2<|z|<3r/2}v(z)\,dz=8b.
$$

The [removable singularity for a bounded harmonic function](../../../../../../removable-singularity-for-a-bounded-harmonic-function.md) fills in the origin, and the [harmonic Liouville theorem](../../../../../../harmonic-liouville-theorem.md) makes the extension constant.

**The conclusion fails for $n\geq3$:** $\boxed{u(x)=|x|^{2-n}}$ is positive and nonconstant, and its radial [Laplacian](../../../../../../laplacian.md) $u''+(n-1)u'/r$ vanishes away from zero. For $n=1$, $\boxed{u(x)=|x|}$ is a nonconstant function bounded below whose second derivative vanishes on both components of the punctured line.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
