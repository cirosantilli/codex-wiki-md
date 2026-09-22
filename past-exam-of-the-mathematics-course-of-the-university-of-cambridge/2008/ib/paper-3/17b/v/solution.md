<h1 id="17b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use real physical fields in the quadratic energy expressions. The vector identity $\nabla\cdot(\mathbf E\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf B)$ and vacuum [Maxwell's equations](../../../../../../maxwell-equations.md) give

$$
\nabla\cdot\left(\frac{\mathbf E\times\mathbf B}{\mu_0}\right)
=-\frac1{\mu_0}\mathbf B\cdot\partial_t\mathbf B-\varepsilon_0\mathbf E\cdot\partial_t\mathbf E
=-\partial_t\left(\frac{\varepsilon_0E^2}{2}+\frac{B^2}{2\mu_0}\right).
$$

Integrating over a fixed volume and applying the [divergence theorem](../../../../../../divergence-theorem.md) proves [Poynting's theorem](../../../../../../poynting-theorem.md):

$$
\boxed{\oint_A\frac{\mathbf E\times\mathbf B}{\mu_0}\cdot d\mathbf A
=-\frac d{dt}\int_V\left(\frac{\varepsilon_0E^2}{2}+\frac{B^2}{2\mu_0}\right)dV.}
$$

The left side is outward energy flux through the closed surface, not merely local intensity.

For a linearly polarized wave with phase $\chi=\mathbf k\cdot\mathbf r-\omega t$, the real fields give [Poynting vector](../../../../../../poynting-vector.md) $\mathbf S=\varepsilon_0cE_0^2\cos^2\chi\,\widehat{\mathbf k}$. Local intensity oscillates at $2\omega$. In the closed-surface integral, the time-independent part cancels because $\oint_A\widehat{\mathbf k}\cdot d\mathbf A=0$. The remaining flux generally oscillates at $2\omega$, has zero time average, and may vanish identically for special volume geometries.

For [circular polarization](../../../../../../circular-polarization.md), take $\mathbf E=E_0(\mathbf e_1\cos\chi+\mathbf e_2\sin\chi)$ with orthonormal transverse vectors. Then $E^2=E_0^2$ and $\mathbf B=\widehat{\mathbf k}\times\mathbf E/c$, so $\mathbf S=\varepsilon_0cE_0^2\widehat{\mathbf k}$ is spatially and temporally constant. Therefore the [closed-surface Poynting flux of a plane wave](../../../../../../closed-surface-poynting-flux-of-a-plane-wave.md) is

$$
\boxed{\oint_A\mathbf S\cdot d\mathbf A=0\quad\text{at every time for circular polarization}.}
$$

There is still a nonzero steady local energy flow: equal energy enters and leaves every fixed closed volume. Calling the net closed-surface flux a nonzero constant would confuse these two quantities.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
