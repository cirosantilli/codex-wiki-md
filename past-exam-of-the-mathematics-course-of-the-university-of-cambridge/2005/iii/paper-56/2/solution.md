<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Enforce the unit-vector constraint using a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\Lambda(x)$:

$$
\widetilde E=\frac12\int\left[\partial_i\phi^a\partial_i\phi^a+
\Lambda(\phi^a\phi^a-1)\right]\,d^2x.
$$

Integration by parts in a compactly supported variation gives $-\Delta\phi^a+\Lambda\phi^a=0$. Contracting with $\phi^a$ gives $\Lambda=\phi^b\Delta\phi^b$, hence

$$
\boxed{\Delta\phi^a-(\phi^b\Delta\phi^b)\phi^a=0.}
$$

Differentiating $\phi^a\phi^a=1$ twice also gives $\phi\cdot\Delta\phi=-|\nabla\phi|^2$, so an equivalent equation is $\Delta\phi+|\nabla\phi|^2\phi=0$. These are the [harmonic map](../../../../../harmonic-map.md) equations for the [O3 nonlinear sigma model](../../../../../o3-nonlinear-sigma-model.md).

For arbitrary maps, the printed finite-energy compactification assertion is too strong. The following counterexample shows that [finite sigma-model energy need not give a limit at infinity](../../../../../finite-sigma-model-energy-need-not-give-a-limit-at-infinity.md). Outside a large disk, set

$$
\phi(r,\vartheta)=(\sin(\log\log r),0,\cos(\log\log r)).
$$

Interpolate smoothly to a constant inside the disk. There is no angular dependence, and the exterior [energy](../../../../../energy.md) is

$$
\frac12\int_{r\geq R}|\nabla\phi|^2\,d^2x
=\pi\int_R^\infty\frac{dr}{r\log^2r}
=\frac{\pi}{\log R}<\infty.
$$

Nevertheless the field keeps rotating and has no limit as $r\to\infty$. Thus [energy](../../../../../energy.md) integrability alone does not prove a continuous map on the [one-point compactification](../../../../../alexandroff-extension.md).

The usual [sigma-model lump](../../../../../sigma-model-lump.md) sector adds the boundary condition $\phi(x)\to\phi_\infty\in S^2$ uniformly as $|x|\to\infty$. Defining the value at the added point to be $\phi_\infty$ then gives a continuous map $S^2\to S^2$: neighborhoods of the point at infinity are precisely complements of compact subsets of the plane, and uniform convergence supplies continuity there. For the [topological degree](../../../../../topological-degree.md) calculation using [differential forms](../../../../../differential-form-split.md) below, take a smooth compactified map, as in the regular lump sector. This boundary/regularity information is additional to finite [energy](../../../../../energy.md) for unrestricted fields.

Write $a_i=\partial_i\phi$ and $b_i=\epsilon_{ij}\phi\times\partial_j\phi$. Since $\phi\cdot\partial_i\phi=0$ and $|\phi|=1$,

$$
\sum_i|b_i|^2=\sum_i|a_i|^2,\qquad
\sum_i a_i\cdot b_i=-2\,\phi\cdot(\partial_1\phi\times\partial_2\phi).
$$

Also the given double-index charge reduces to

$$
Q=\frac1{4\pi}\int
\phi\cdot(\partial_1\phi\times\partial_2\phi)\,d^2x.
$$

For $s=\pm1$, expanding the nonnegative square gives

$$
\int\sum_i|a_i+s b_i|^2\,d^2x=4E-16\pi sQ.
$$

Therefore the [Bogomolny degree bound for the O3 sigma model](../../../../../bogomolny-degree-bound-for-the-o3-sigma-model.md) is

$$
\boxed{E\geq4\pi|Q|.}
$$

The charge integral is absolutely convergent already for finite-energy fields, because $|\phi\cdot(\partial_1\phi\times\partial_2\phi)|\leq\frac12(|\partial_1\phi|^2+|\partial_2\phi|^2)$. The inequality itself consequently does not need the compactification hypothesis. Equality requires $\partial_i\phi+s\epsilon_{ij}\phi\times\partial_j\phi=0$ for $s$ chosen to have the sign of $Q$.

For the topological interpretation, the standard oriented area form on the target [sphere](../../../../../sphere.md) is

$$
\omega=\frac12\epsilon_{abc}y^a\,dy^b\wedge dy^c,\qquad
\int_{S^2}\omega=4\pi.
$$

Its pullback is $\phi^*\omega=\phi\cdot(\partial_1\phi\times\partial_2\phi)\,dx^1\wedge dx^2$. The [topological degree](../../../../../topological-degree.md) is defined by $\phi_*[S^2]=\deg(\phi)[S^2]$ in $H_2(S^2;\mathbb Z)\cong\mathbb Z$. Pairing with $\omega$ gives

$$
\int_{S^2}\phi^*\omega=\deg(\phi)\int_{S^2}\omega,
\qquad
\boxed{Q=\deg(\phi)\in\mathbb Z.}
$$

Equivalently, the integer is the signed number of preimages of a regular value. It is invariant under smooth [homotopy](../../../../../homotopy.md): if $\Phi:S^2\times[0,1]\to S^2$ is that [homotopy](../../../../../homotopy.md), then [Stokes theorem](../../../../../stokes-theorem.md) and $d\omega=0$ make the difference between the two charge integrals equal to $\int_{S^2\times[0,1]}d(\Phi^*\omega)=0$. This identifies the charge as the [degree charge of an O3 sigma-model lump](../../../../../degree-charge-of-an-o3-sigma-model-lump.md), rather than merely an arbitrary [energy](../../../../../energy.md) integral.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
