<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $m$ be the sliding [point charge](../../../../point-charge.md)'s [mass](../../../../mass.md). Expanding the [axial field of a uniformly charged annulus](../../../../axial-field-of-a-uniformly-charged-annulus.md) for $|x|\ll a,b$ gives

$$
E_x=\frac{\sigma}{2\epsilon_0}\left(\frac1a-\frac1b\right)x+O(x^3)
=\frac{Q}{2\pi\epsilon_0ab(a+b)}x+O(x^3).
$$

Its [electric charge](../../../../electric-charge-split.md) is $-Q$, so its [electric force](../../../../electric-force.md) points toward the centre. [Newton's second law](../../../../newton-s-second-law.md) becomes

$$
m\ddot x=-\frac{Q^2}{2\pi\epsilon_0ab(a+b)}x+O(x^3).
$$

To leading order this is [simple harmonic motion](../../../../simple-harmonic-motion.md), with

$$
\boxed{\omega_{\rm osc}^2=\frac{Q^2}{2\pi\epsilon_0mab(a+b)},\qquad
T=2\pi\sqrt{\frac{2\pi\epsilon_0mab(a+b)}{Q^2}}.}
$$

The [mass](../../../../mass.md) is an additional parameter, since the source supplies no numerical value. The constraint is essential: [stability](../../../../stability-of-a-numerical-method.md) along the axis does not imply unconstrained three-dimensional trapping by a static [electric field](../../../../electric-field-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
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
