<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [geometrized units](../../../../../geometrized-units.md) and assume $M>0$, $|Q|\le M$, so the [Reissner-Nordstrom spacetime](../../../../../reissner-nordstrom-spacetime.md) contains a [black hole](../../../../../black-hole.md). Its outer [event horizon](../../../../../event-horizon.md) is $r_+=M+\sqrt{M^2-Q^2}$. The classical absorption cross-section is obtained in [geometrical optics](../../../../../geometrical-optics.md), by counting incident [null geodesics](../../../../../null-geodesic.md) captured from infinity. Spherical symmetry lets us use the equatorial plane. Write $f(r)=1-2M/r+Q^2/r^2$, and let a dot denote differentiation with respect to an affine parameter. The conserved [Killing energy](../../../../../killing-energy.md) and angular momentum are $E=f\dot t$ and $L=r^2\dot\phi$. Null normalization gives

$$
0=-f\dot t^2+f^{-1}\dot r^2+r^2\dot\phi^2,\qquad
\dot r^2=E^2-L^2\frac{f(r)}{r^2}=E^2\left(1-b^2W(r)\right),
$$

where the [impact parameter](../../../../../impact-parameter.md) is $b=L/E$ and $W=f/r^2$. An incoming ray turns around if the angular-momentum barrier reaches $E^2$ before the ray reaches the [event horizon](../../../../../event-horizon.md). The limiting captured ray approaches the exterior unstable [circular null geodesic](../../../../../circular-null-geodesic.md), at the maximum of $W$.

The stationary-point equation is

$$
W'(r)=-\frac{2}{r^5}\left(r^2-3Mr+2Q^2\right)=0.
$$

The outer root is the [photon sphere](../../../../../photon-sphere.md) radius

$$
\boxed{r_{\mathrm{ph}}=\frac{3M+\sqrt{9M^2-8Q^2}}2.}
$$

It lies outside $r_+$: for $|Q|\le M$ it ranges from $3M$ down to $2M$, whereas $r_+$ ranges from $2M$ down to $M$. More precisely $r_{\mathrm{ph}}>2M$ except in the extremal case, and $r_+\le2M$; even at extremality $r_{\mathrm{ph}}=2M>r_+=M$. At this root,

$$
W''(r_{\mathrm{ph}})=-\frac{2(2r_{\mathrm{ph}}-3M)}{r_{\mathrm{ph}}^5}<0,
$$

so the [circular null geodesic](../../../../../circular-null-geodesic.md) is unstable. The smaller stationary root lies at or inside the outer horizon and does not set capture from infinity. For $b<b_c$, the radial equation has no exterior turning point and the ray enters the [event horizon](../../../../../event-horizon.md); for $b>b_c$, it turns around. The critical [impact parameter](../../../../../impact-parameter.md) is therefore

$$
b_c^2=\frac1{W(r_{\mathrm{ph}})}=\frac{r_{\mathrm{ph}}^2}{f(r_{\mathrm{ph}})}.
$$

The stationary-point equation gives $Q^2=(3Mr_{\mathrm{ph}}-r_{\mathrm{ph}}^2)/2$, hence $f(r_{\mathrm{ph}})=(r_{\mathrm{ph}}-M)/(2r_{\mathrm{ph}})$. Since a parallel incident beam is captured over a disk of radius $b_c$, the [photon capture cross-section of a Reissner-Nordstrom black hole](../../../../../photon-capture-cross-section-of-a-reissner-nordstrom-black-hole.md) is

$$
\boxed{\sigma_{\mathrm{abs}}=\pi b_c^2
=\frac{2\pi r_{\mathrm{ph}}^3}{r_{\mathrm{ph}}-M}
=\frac{\pi\left(3M+\sqrt{9M^2-8Q^2}\right)^3}{2\left(M+\sqrt{9M^2-8Q^2}\right)}.}
$$

The equality case approaches the unstable orbit indefinitely, but it is a measure-zero boundary of the captured disk and does not change the cross-section.

For the suggested parameterization, choose $\psi$ with $Q=3M\sin\psi/\sqrt8$ and $\cos\psi\ge0$. Then $\sqrt{9M^2-8Q^2}=3M\cos\psi$, so the same cross-section is

$$
\boxed{\sigma_{\mathrm{abs}}=\frac{27\pi M^2}{2}\frac{(1+\cos\psi)^3}{1+3\cos\psi}.}
$$

The black-hole range has $|\sin\psi|\le\sqrt8/3$, hence $\cos\psi\ge1/3$. For $Q=0$, $r_{\mathrm{ph}}=3M$, $f(r_{\mathrm{ph}})=1/3$, and $b_c=3\sqrt3M$, giving

$$
\boxed{\sigma_{\mathrm{abs}}(Q=0)=27\pi M^2,}
$$

the classical [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md) light-capture result. As an additional limit check, $|Q|=M$ gives $r_{\mathrm{ph}}=2M$, $b_c=4M$, and $\sigma_{\mathrm{abs}}=16\pi M^2$. These are geometric capture areas, larger than the corresponding horizon areas; the relevant barrier is the [photon sphere](../../../../../photon-sphere.md), not the horizon's apparent disk. The result applies to light in the short-[wavelength](../../../../../wavelength.md) limit, while a finite-frequency wave absorption cross-section depends on the [greybody factors](../../../../../greybody-factor.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
