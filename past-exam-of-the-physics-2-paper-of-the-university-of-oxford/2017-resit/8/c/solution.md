<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [electric dipole above a grounded conducting plane](../../../../electric-dipole-above-a-grounded-conducting-plane.md) approximation, valid for $d\ll a$. Let $\hat{\mathbf z}$ point upward, and choose $\mathbf p=p(\sin\theta\,\hat{\mathbf x}+\cos\theta\,\hat{\mathbf z})$. Reflecting the two constituent [point charges](../../../../point-charge.md) and reversing their signs produces an image [electric dipole moment](../../../../electric-dipole-moment.md)

$$
\mathbf p'=p(-\sin\theta\,\hat{\mathbf x}+\cos\theta\,\hat{\mathbf z})
$$

at height $-a$. Thus the parallel [electric dipole moment](../../../../electric-dipole-moment.md) reverses and the normal one is unchanged. At the real [electric dipole](../../../../electric-dipole.md), the separation from its image is $2a\hat{\mathbf z}$, giving the image [electric field](../../../../electric-field-split.md)

$$
\mathbf E_{\rm im}=\frac{1}{4\pi\epsilon_0(2a)^3}
\left[3(\mathbf p'\cdot\hat{\mathbf z})\hat{\mathbf z}-\mathbf p'\right]
=\frac{p}{32\pi\epsilon_0a^3}
\left(\sin\theta\,\hat{\mathbf x}+2\cos\theta\,\hat{\mathbf z}\right).
$$

The physical [torque](../../../../torque.md) is $\boldsymbol\tau=\mathbf p\times\mathbf E_{\rm im}$, so

$$
\boxed{\boldsymbol\tau=-\frac{p^2\sin\theta\cos\theta}{32\pi\epsilon_0a^3}\hat{\mathbf y}
=-\frac{p^2\sin2\theta}{64\pi\epsilon_0a^3}\hat{\mathbf y}.}
$$

For $0<\theta<\pi/2$, its direction reduces $\theta$, tending to align the [electric dipole](../../../../electric-dipole.md) with the upward normal. In general it favours either normal orientation; a perfectly parallel orientation has zero [torque](../../../../torque.md) but is unstable to tilting.

The conductor-response [potential energy](../../../../potential-energy.md) includes one half of the real-image interaction:

$$
U=-\frac12\mathbf p\cdot\mathbf E_{\rm im}
=-\frac{p^2(1+\cos^2\theta)}{64\pi\epsilon_0a^3}.
$$

This factor accounts for the induced [surface charge](../../../../surface-charge.md) changing as the physical source is assembled. Differentiation with respect to height at fixed orientation gives

$$
\boxed{\mathbf F=-\frac{\partial U}{\partial a}\hat{\mathbf z}
=-\frac{3p^2(1+\cos^2\theta)}{64\pi\epsilon_0a^4}\hat{\mathbf z}.}
$$

There is no horizontal [force](../../../../force-split.md), since translating the entire arrangement parallel to the plane leaves $U$ unchanged. For example, the normal and parallel orientations give respective downward [force](../../../../force-split.md) magnitudes $3p^2/(32\pi\epsilon_0a^4)$ and $3p^2/(64\pi\epsilon_0a^4)$.

A single physical [point charge](../../../../point-charge.md) induces total plane [electric charge](../../../../electric-charge-split.md) $-q$. One can verify this by integrating its induced [surface charge density](../../../../surface-charge-density.md), $-qh/[2\pi(\varrho^2+h^2)^{3/2}]$, over the plane. The two physical [electric charges](../../../../electric-charge-split.md) therefore induce opposite totals, giving

$$
\boxed{Q_{\rm plane}=-(+q)-(-q)=0.}
$$

The local [surface charge density](../../../../surface-charge-density.md) is generally nonzero. The zero total holds for the finite neutral pair as well as its ideal [electric dipole](../../../../electric-dipole.md) limit.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
