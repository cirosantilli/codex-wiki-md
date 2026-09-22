<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

Take $\theta$ as the inclination of the symmetry axis to the upward vertical, $\phi$ as its azimuth, and $\psi$ as rotation of the body about that axis relative to the line of nodes. The [kinetic energy](../../../../../kinetic-energy.md) and [potential energy](../../../../../potential-energy.md) are

$$
T=\frac A2(\dot\theta^2+\dot\phi^2\sin^2\theta)+\frac C2(\dot\psi+\dot\phi\cos\theta)^2,\qquad V=mg\ell\cos\theta.
$$

The [cyclic coordinates](../../../../../cyclic-coordinate.md) $\psi,\phi$ and time independence give three conserved quantities:

$$
L=C(\dot\psi+\dot\phi\cos\theta),\qquad
p_\phi=A\dot\phi\sin^2\theta+L\cos\theta,\qquad E=T+V.
$$

Their meanings are the component of [angular momentum](../../../../../angular-momentum.md) along the body axis, the component along the vertical, and the total [energy](../../../../../energy.md).

For a vanishingly small perturbation of the upright spinning state, $L\simeq Cn$, $p_\phi\simeq L$, and $E\simeq L^2/(2C)+mg\ell$. Eliminating $\dot\phi$ gives the limiting [effective potential](../../../../../effective-potential.md)

$$
U_{\rm eff}(\theta)=\frac{L^2}{2A}\tan^2(\theta/2)+\frac{L^2}{2C}+mg\ell\cos\theta.
$$

Its quadratic change near zero is $\{L^2/(8A)-mg\ell/2\}\theta^2$. Thus if **$C^2n^2>4mg\ell A$**, zero is a strict local minimum and a sufficiently small perturbation remains near it.

In the unstable case, the limiting energy equation becomes

$$
\frac A2\dot\theta^2=(1-\cos\theta)\left[mg\ell-\frac{L^2}{2A(1+\cos\theta)}\right].
$$

At the nonzero turning point the bracket vanishes, yielding

$$
\boxed{\cos\theta_{\max}\simeq\frac{C^2n^2}{2mg\ell A}-1}.
$$

The approximation is the small-perturbation limit, not an assertion that arbitrary disturbances preserve the upright state's exact conserved quantities.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
