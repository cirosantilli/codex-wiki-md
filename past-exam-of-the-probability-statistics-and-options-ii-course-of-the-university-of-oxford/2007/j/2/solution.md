<h1 id="j/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In vacuum, the source-free [Maxwell equations](../../../../maxwell-equations-split.md) are

$$
\nabla\cdot\mathbf E=\nabla\cdot\mathbf B=0,\qquad
\nabla\times\mathbf E=-\partial_t\mathbf B,\qquad
\nabla\times\mathbf B=c^{-2}\partial_t\mathbf E.
$$

Put $\psi=\omega(t-z/c)$ and denote the constant electric amplitude by $E_0$. A corresponding traveling-wave [magnetic field](../../../../magnetic-field-split.md) is

$$
\boxed{\mathbf B=\frac{E_0}{c}(-\sin\psi,\cos\psi,0).}
$$

Both [divergences](../../../../divergence.md) vanish because both the [electric field](../../../../electric-field-split.md) and the [magnetic field](../../../../magnetic-field-split.md) depend only on $z,t$ and have zero $z$ component. Direct differentiation gives $\nabla\times\mathbf E=(\omega E_0/c)(\cos\psi,\sin\psi,0)=-\partial_t\mathbf B$ and $\nabla\times\mathbf B=(\omega E_0/c^2)(-\sin\psi,\cos\psi,0)=c^{-2}\partial_t\mathbf E$. A time-independent background [magnetic field](../../../../magnetic-field-split.md) satisfying the homogeneous equations could be added; the formula is the wave component.

Introduce the [magnetic vector potential](../../../../magnetic-vector-potential.md) and [electric potential](../../../../electric-potential.md) by $\mathbf B=\nabla\times\mathbf A$ and $\mathbf E=-\nabla\phi-\partial_t\mathbf A$. These identities automatically give the divergence equation for $\mathbf B$ and [Faraday's law](../../../../faraday-s-law-of-induction.md). For this wave choose $\phi=0$ and $\mathbf A=(c/\omega)\mathbf B$; the [derivatives](../../../../derivative.md) just calculated verify both potential equations.

The electromagnetic [force](../../../../force-split.md) is the [Lorentz force](../../../../lorentz-force.md), $Q(\mathbf E+\mathbf v\times\mathbf B)$. On the smooth constraint plane $z=z_0$, the [constraint force](../../../../constraint-force.md) is normal to the plane. Both $\mathbf v$ and $\mathbf B$ are tangential, so $\mathbf v\times\mathbf B$ is normal and is balanced by that [constraint force](../../../../constraint-force.md); it does not affect the tangential motion. Thus

$$
\ddot{\mathbf r}_\parallel=\frac{QE_0}{m}(\cos\psi,\sin\psi).
$$

A particular motion is $\mathbf r_\parallel=\mathbf r_0-[QE_0/(m\omega^2)](\cos\psi,\sin\psi)$, a circle of radius

$$
\boxed{\frac{|QE_0|}{m\omega^2}.}
$$

The general planar motion also includes a constant drift [velocity](../../../../velocity.md); the particle moves on a circle when that drift is zero. The [constraint force](../../../../constraint-force.md) can do no work because it is perpendicular to the [velocity](../../../../velocity.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [J](../../j.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
