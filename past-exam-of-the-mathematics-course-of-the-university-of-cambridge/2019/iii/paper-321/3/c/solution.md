<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [horizontally invariant magnetized shearing-sheet equations](../../../../../../horizontally-invariant-magnetized-shearing-sheet-equations.md) are linear in the horizontal fields, so perturbations about the equilibrium satisfy the same equations. The fixed surface [boundary conditions](../../../../../../boundary-condition.md) require $\delta B_x=\delta B_y=0$ at $z=\pm H$. Choose a [normal mode](../../../../../../normal-mode.md) with

$$
(\delta B_x,\delta B_y)=(b_x,b_y)e^{st}\sin[k(z+H)],\qquad
(\delta v_x,\delta v_y)=(u,v)e^{st}\cos[k(z+H)],
$$

where the [vertical wavenumber](../../../../../../vertical-wavenumber.md) is $k=m\pi/(2H)$, $m=1,2,\ldots$. With the [Alfvén frequency](../../../../../../alfven-frequency.md)

$$
\omega_a^2=\frac{k^2B_z^2}{\mu_0\rho}=k^2v_{Az}^2,
$$

the four amplitude equations become

$$
su-2\Omega v=\frac{kB_z}{\mu_0\rho}b_x,\qquad
sv+(2-q)\Omega u=\frac{kB_z}{\mu_0\rho}b_y,
$$



$$
sb_x=-kB_zu,\qquad sb_y+q\Omega b_x=-kB_zv.
$$

Eliminating the velocities leaves

$$
(s^2+\omega_a^2-2q\Omega^2)b_x-2\Omega s b_y=0,\qquad
2\Omega s b_x+(s^2+\omega_a^2)b_y=0.
$$

A nonzero amplitude requires the [determinant](../../../../../../determinant.md) of this system to vanish, yielding the [ideal magnetorotational dispersion relation](../../../../../../ideal-magnetorotational-dispersion-relation.md)

$$
\boxed{(s^2+\omega_a^2)(s^2+\omega_a^2-2q\Omega^2)+4\Omega^2s^2=0}.
$$

Equivalently, with $\kappa_r^2=2(2-q)\Omega^2$,

$$
s^4+(2\omega_a^2+\kappa_r^2)s^2+\omega_a^2(\omega_a^2-2q\Omega^2)=0.
$$

As a [quadratic equation](../../../../../../quadratic-equation.md) for $s^2$, its [discriminant](../../../../../../discriminant.md) is $\kappa_r^4+16\Omega^2\omega_a^2>0$. If $0<\omega_a^2<2q\Omega^2$, its constant term is negative, so one root $s^2$ is positive and there is an exponentially growing mode. If $\omega_a^2>2q\Omega^2$, both the constant term and the coefficient of $s^2$ are positive, giving two negative roots and only oscillatory modes. Equality is marginal.

The lowest allowed [vertical wavenumber](../../../../../../vertical-wavenumber.md), $k=\pi/(2H)$, is the last to be stabilized as $|B_z|$ increases. Therefore the [finite-thickness magnetorotational instability criterion](../../../../../../finite-thickness-magnetorotational-instability-criterion.md) is

$$
\boxed{0<\frac{\pi^2B_z^2}{8q\mu_0\rho H^2\Omega^2}<1}.
$$

There is also a vertically uniform velocity mode with zero magnetic perturbation; for the usual orbitally stable regime $q<2$, it is just stable [epicyclic motion](../../../../../../epicyclic-motion.md). For $q>2$, that uniform mode is already hydrodynamically unstable, independently of the magnetic criterion. At $q=2$ it is marginal. The criterion above concerns the magnetic modes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
