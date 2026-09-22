<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Roche lobe](../../../../../../roche-lobe.md) of star 1 is the volume around it bounded by the critical closed equipotential passing through the inner [Lagrange point](../../../../../../lagrange-point.md) $L_1$. Material on a lower potential surface remains confined to star 1; at the critical surface a path opens toward star 2.

Let $\mathbf g=-\nabla\Psi$ and take $d\mathbf S$ outward. For a nearly spherical interior surface, the [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
\int_S\mathbf g\mathbin\cdot d\mathbf S
=-\int_V\nabla^2\Psi\,dV.
$$

The self-gravity term contributes $-4\pi GM_1$. The companion lies outside $S$, so its potential is harmonic inside and contributes zero net flux. For the centrifugal term, $\nabla^2(-\Omega^2s^2/2)=-2\Omega^2$, so its acceleration has divergence $2\Omega^2$ and contributes $2\Omega^2V$. Using $V=4\pi r^3/3$ and $S=4\pi r^2$,

$$
\boxed{
\langle g\rangle
=\frac1S\int_S\mathbf g\mathbin\cdot d\mathbf S
\simeq-\frac{GM_1}{r^2}+\frac23\Omega^2r}.
$$

The sign is the outward-normal component; the dominant self-gravity is inward and therefore negative.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
