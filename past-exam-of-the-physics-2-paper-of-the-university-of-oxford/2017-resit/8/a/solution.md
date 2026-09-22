<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $\mathbf d$ from the negative to the positive [point charge](../../../../point-charge.md). Their [electric dipole moment](../../../../electric-dipole-moment.md) is $\mathbf p=q\mathbf d$. Place them at $\pm\mathbf d/2$ and use the [superposition principle](../../../../superposition-principle.md) for the [electric potential](../../../../electric-potential.md):

$$
V(\mathbf s)=\frac{q}{4\pi\epsilon_0}
\left(\frac1{|\mathbf s-\mathbf d/2|}-\frac1{|\mathbf s+\mathbf d/2|}\right).
$$

For $s\gg d$, the first-order [Taylor expansion](../../../../taylor-expansion.md) of the reciprocal distances gives

$$
\boxed{V(s,\theta)=\frac{\mathbf p\cdot\hat{\mathbf s}}{4\pi\epsilon_0s^2}
=\frac{p\cos\theta}{4\pi\epsilon_0s^2}}
$$

to leading [electric dipole](../../../../electric-dipole.md) order. In [spherical coordinates](../../../../spherical-coordinate-system.md) aligned with $\mathbf p$, the [gradient](../../../../gradient.md) gives $E_s=-\partial_sV$, $E_\theta=-s^{-1}\partial_\theta V$ and $E_\phi=0$. Thus

$$
\boxed{\mathbf E(s,\theta)=\frac{p}{4\pi\epsilon_0s^3}
\left(2\cos\theta\,\hat{\mathbf s}+\sin\theta\,\hat{\boldsymbol\theta}\right).}
$$

Equivalently, the [electric dipole field](../../../../electric-dipole-field.md) is $[3(\mathbf p\cdot\hat{\mathbf s})\hat{\mathbf s}-\mathbf p]/(4\pi\epsilon_0s^3)$. The omitted terms vanish relative to these leading expressions as $d/s\to0$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
