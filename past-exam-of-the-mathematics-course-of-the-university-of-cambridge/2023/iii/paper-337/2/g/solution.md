<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Choose the orientation of spherical coordinates as

$$
\widetilde{\mathbf n}
=(\sin\theta\cos\phi,-\sin\theta\sin\phi,\cos\theta),
$$

which differs from the opposite azimuth convention only by $\phi\mapsto-\phi$. With $\mathbf B=B\widehat{\mathbf x}$, $\theta=\pi/2-\delta\theta$, and $\phi=\delta\phi$,

$$
\widetilde{\mathbf n}
=(1,-\delta\phi,\delta\theta)+O(\delta^2).
$$

Substitution into the effective action gives

$$
\boxed{
\mathcal L_{eff}
=-\alpha^2\left[(\nabla\delta\theta)^2
+(\nabla\delta\phi)^2\right]
+\beta^2\left[(\partial_t\delta\theta+B\delta\phi)^2
+(\partial_t\delta\phi-B\delta\theta)^2\right],}
$$

where

$$
\boxed{\alpha^2=\frac{JS^2}{2},
\qquad
\beta^2=\frac1{16Ja^2}.}
$$

Let $\psi=\delta\theta+i\delta\phi$ and define the zero-field [spin-wave velocity](../../../../../../spin-wave-velocity.md)

$$
c=\frac\alpha\beta=2\sqrt2\,JSa.
$$

The linearized equation is

$$
(\partial_t-iB)^2\psi-c^2\nabla^2\psi=0.
$$

For a plane wave, the two circular polarizations therefore obey

$$
\boxed{(\omega\pm B)^2=c^2k^2,}
$$

or, with signed-frequency branches, $\omega=ck\pm B$ and their negative-frequency partners. At $B=0$ these are the two degenerate, linearly dispersing [antiferromagnetic spin waves](../../../../../../antiferromagnetic-spin-wave.md). The field [Zeeman-splits](../../../../../../zeeman-splitting.md) the two opposite circular polarizations by shifting their frequencies in opposite directions.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
