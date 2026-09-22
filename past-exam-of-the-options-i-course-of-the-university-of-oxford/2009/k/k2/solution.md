<h1 id="k/k2/solution">Solution</h1>

↑ **Parent:** [K2](../k2.md)

For the isolated [line vortex](../../../../line-vortex.md), use [polar coordinates](../../../../polar-coordinates.md) $z=re^{i\theta}$ to obtain

$$
\phi=\frac\Gamma{2\pi}\theta,\qquad
\psi=-\frac\Gamma{2\pi}\log r,\qquad
u_r=0,\quad u_\theta=\frac\Gamma{2\pi r}.
$$

Thus for nonzero $\Gamma$ the [streamlines](../../../../streamline.md) are circles and their counterclockwise [circulation](../../../../circulation-physics.md) is $2\pi r u_\theta=\Gamma$. If $\Gamma=0$ the fluid is stationary and the [streamline](../../../../streamline.md) description degenerates.

Place an opposite image [vortex](../../../../phase-vortex.md) at $z=-1$. The [method of images](../../../../method-of-images.md) gives

$$
\boxed{w(z)=-\frac{i\Gamma}{2\pi}\bigl(\log(z-1)-\log(z+1)\bigr)}.
$$

On $z=iy$, the distances to the two [vortex](../../../../phase-vortex.md) positions agree, so $\psi=-(\Gamma/2\pi)\log(|z-1|/|z+1|)=0$. Hence the wall is a [streamline](../../../../streamline.md). Directly the wall velocity has $u=0$ and

$$
v(0,y)=-\frac\Gamma{\pi(1+y^2)}.
$$

For the stipulated steady flow, [Bernoulli's equation](../../../../bernoulli-equation.md) in the irrotational fluid outside the [vortex](../../../../phase-vortex.md) core gives

$$
p(0,y)-p_\infty=-\frac12\rho v(0,y)^2
=-\frac{\rho\Gamma^2}{2\pi^2(1+y^2)^2}.
$$

The force exerted by the fluid on this wall points in the $-x$ direction for positive [pressure](../../../../pressure-split.md). Relative to uniform [pressure](../../../../pressure-split.md) $p_\infty$, however, its change is in the $+x$ direction. Using the supplied integral, the force change per unit span is

$$
\boxed{\Delta\mathbf F_{\rm wall}=\frac{\rho\Gamma^2}{4\pi}\,\mathbf e_x}.
$$

Thus the wall is attracted **towards the [vortex](../../../../phase-vortex.md)**, with this magnitude if the other side remains at $p_\infty$. Subtracting the uniform [pressure](../../../../pressure-split.md) is essential for an infinite wall. A freely moving [vortex](../../../../phase-vortex.md) would translate parallel to the wall under its image-induced velocity; the calculation here is for the stated steady [vortex](../../../../phase-vortex.md) configuration, with its position held fixed.

## ↑ Ancestors (12)

1. [K2](../k2.md)
2. [K](../../k.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
