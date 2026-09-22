<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**False.** The enclosed-mass formula is a consequence of the [spherical shell theorem](../../../../../../spherical-shell-theorem.md). In a spherical [galaxy](../../../../../../galaxy-split.md), exterior shells exert no radial force and interior mass acts as though concentrated at the centre, giving $v_c^2=GM(<r)/r$.

A razor-thin axisymmetric disc instead has

$$
\boxed{v_c^2(R)=R\,\partial_R\Phi(R,0)=-R\,\partial_R\psi(R,0).}
$$

Both interior and exterior annuli contribute to that derivative. Its geometry is not determined by $M(<R)$.

A concrete counterexample compares a central point mass $M_0$ plus an exterior spherical shell with the same point mass plus a thin circular ring of mass $m$ and radius $a$. Their enclosed-mass profiles are identical: $M_0$ inside $a$, and $M_0+m$ outside. The [interior gravitational force of an exterior thin ring](../../../../../../interior-gravitational-force-of-an-exterior-thin-ring.md) follows by expanding its angularly averaged relative potential:

$$
\psi_{\mathrm{ring}}(R)=\frac{Gm}{2\pi}\int_0^{2\pi}\frac{d\varphi}{\sqrt{a^2+R^2-2aR\cos\varphi}}=\frac{Gm}{a}\left[1+\frac{R^2}{4a^2}+O\left(\frac{R^4}{a^4}\right)\right].
$$

For $R\ll a$, the ring's acceleration is outward, $\partial_R\psi_{\mathrm{ring}}=GmR/(2a^3)+\cdots$, whereas the spherical shell's acceleration is zero. With $M_0$ large enough to retain [circular orbits](../../../../../../circular-orbit.md), the disc-side speed is

$$
\boxed{v_{c,\mathrm{ring}}^2=\frac{GM_0}{R}-\frac{GmR^2}{2a^3}+\cdots\ne\frac{GM_0}{R}=v_{c,\mathrm{sphere}}^2.}
$$

A narrow smooth annulus gives the same distinction. This proves that [enclosed mass does not determine a disc rotation curve](../../../../../../enclosed-mass-does-not-determine-a-disc-rotation-curve.md), even when the mass profiles of the spherical and disc models agree.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
