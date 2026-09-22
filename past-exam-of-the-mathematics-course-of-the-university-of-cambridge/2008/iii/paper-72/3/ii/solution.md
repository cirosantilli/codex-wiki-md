<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An orbital prescription is needed to fix the coefficient in a [tidal radius](../../../../../../tidal-radius.md). Adopt a low-mass satellite on a circular orbit of separation $D$, with $r_t\ll D$. The host [singular isothermal sphere](../../../../../../singular-isothermal-sphere.md) has

$$
\Phi_h'(D)=\frac{2\sigma_h^2}{D},\qquad \Phi_h''(D)=-\frac{2\sigma_h^2}{D^2},\qquad \Omega^2=\frac{\Phi_h'(D)}D=\frac{2\sigma_h^2}{D^2}.
$$

In the corotating frame, subtract the host force on the satellite centre and add the differential centrifugal force. Along the line joining the centres, the outward effective acceleration to first order in displacement $r$ is $(\Omega^2-\Phi_h'')r=4\sigma_h^2r/D^2$. Equate this to the dwarf's inward acceleration at its edge:

$$
\frac{Gm_d(<r_t)}{r_t^2}=\frac{2\sigma_d^2}{r_t}=\frac{4\sigma_h^2r_t}{D^2}.
$$

This gives the [Jacobi truncation of two singular isothermal spheres](../../../../../../jacobi-truncation-of-two-singular-isothermal-spheres.md)

$$
\boxed{r_t=\frac{D\sigma_d}{\sqrt2\sigma_h}.}
$$

It is the distance to the radial escape saddle, not an exact spherical surface: the actual tidal lobe is distorted. For an eccentric orbit, separation alone does not specify an instantaneous effective angular speed or the stripping history; a pericentric estimate is commonly used with further assumptions.

A simpler order-of-magnitude convention equates mean internal and host densities, $m_d/r_t^3=M_h(D)/D^3$, giving $r_t\sim D\sigma_d/\sigma_h$. Equivalently it retains the host gradient without the circular-orbit centrifugal contribution. Both reproduce the scaling $r_t\propto D\sigma_d/\sigma_h$, but their coefficients differ by $\sqrt2$. The familiar point-mass factor three is not appropriate for this extended host, whose enclosed mass grows linearly with radius. The circular-orbit [Jacobi tidal radius](../../../../../../jacobi-tidal-radius.md) will be used consistently below, with the rough convention's numerical values also given.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
