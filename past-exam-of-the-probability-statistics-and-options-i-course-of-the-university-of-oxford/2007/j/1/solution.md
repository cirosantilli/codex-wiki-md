<h1 id="j/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a consistently oriented surface and boundary, [Ampère's law](../../../../ampere-s-circuital-law.md) is

$$
\oint_\Gamma\mathbf B\cdot d\boldsymbol\ell
=\mu_0 I_{\rm enc}
=\mu_0\int_S\mathbf J\cdot\mathbf n\,dS.
$$

[Stokes theorem](../../../../stokes-theorem.md) gives the left side as $\int_S(\nabla\times\mathbf B)\cdot\mathbf n\,dS$, so the given [curl](../../../../curl.md) equation proves the law.

On a circle of radius $r$ around the axis, the assumed azimuthal field is tangent and constant in magnitude. Thus the [circulation](../../../../circulation-physics.md) is $2\pi rB_\theta(r)$. For $r\leq a$, the enclosed [electric current](../../../../electric-current.md) is $I r^2/a^2$; for $r\geq a$, it is $I$. Therefore

$$
\boxed{\mathbf B(r)=
\begin{cases}
\dfrac{\mu_0 I r}{2\pi a^2}\mathbf e_\theta,&0\leq r\leq a,\\[4pt]
\dfrac{\mu_0 I}{2\pi r}\mathbf e_\theta,&r\geq a.
\end{cases}}
$$

The field is continuous at $r=a$ and vanishes regularly at the axis. Its direction follows the right-hand rule for positive [electric current](../../../../electric-current.md) along $\mathbf e_z$. The radial component of the [curl](../../../../curl.md) equation also gives $\partial_zB_\theta=0$, so the expression is valid at every height; no unmentioned axial dependence remains.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [J](../../j.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
