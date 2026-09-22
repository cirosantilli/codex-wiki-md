<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\psi=B_1/B_2$. The middle layer matches the density of plume 1 at $h_1$, so $g_1'=B_1/q_1$. The upper layer exports both sources, so $g_2'=(B_1+B_2)/Q$. With $Q=q_1+q_{21}$ and $q_{21}/q_1=\psi^{-1/3}$, the [two-plume three-layer displacement ventilation](../../../../../../two-plume-three-layer-displacement-ventilation.md) density ratio is

$$
\boxed{\frac{\Delta\rho_1}{\Delta\rho_2}=\frac{g_1'}{g_2'}
=\frac{\psi+\psi^{2/3}}{1+\psi}.}
$$

The driving head can therefore be rewritten as $\mathcal H=g_2'\mathcal L$, where

$$
\mathcal L=H-h_1-\frac{1-\psi^{2/3}}{1+\psi}(h_2-h_1).
$$

Combining $Q^2=(A^*)^2g_2'\mathcal L$ with $g_2'Q=B_2(1+\psi)$ gives $Q^3=(A^*)^2B_2(1+\psi)\mathcal L$. But $Q^3=C^3B_2(1+\psi^{1/3})^3h_1^5$, and hence

$$
\boxed{\frac{A^*}{H^2C^{3/2}}
=\frac{(1+\psi^{1/3})^{3/2}}{(1+\psi)^{1/2}}
\left[\frac{(h_1/H)^5}
{1-h_1/H-\frac{1-\psi^{2/3}}{1+\psi}(h_2-h_1)/H}\right]^{1/2}.}
$$

The square root requires a positive remaining buoyancy head.

As $\psi\to0$, the weak source vanishes and $g_1'/g_2'\to0$: the middle and lower layers have the same density, leaving a single physical interface at $h_2$. The old $h_1$ no longer marks an independent density interface. The single-plume two-layer model is the meaningful limit; the additional closure in part (e) also gives $h_2/h_1\to1$.

As $\psi\to1$, the density ratio tends to one, so the middle and upper layers merge. There is then a single physical lower interface $h_1$, fed by two equal, separate plumes. The area prefactor tends to two and the head reduces to $g'(H-h_1)$. The mathematical label $h_2$ ceases to identify a distinct density interface, so a finite limiting value assigned to it by an extra closure is not evidence for three distinct layers. Two separate equal plumes entrain more than one coincident plume of combined source strength; the distinction survives after the layers merge.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
