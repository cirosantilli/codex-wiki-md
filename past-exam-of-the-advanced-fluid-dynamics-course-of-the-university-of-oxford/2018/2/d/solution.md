<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The undisturbed ambient solution is smooth and free of [body forces](../../../../body-force.md) throughout the ball $r\le a$. Its [Stokes equations](../../../../stokes-equation.md) imply

$$
\mu\nabla^2\mathbf u_\infty=\nabla p_\infty,\qquad
\nabla\cdot\mathbf u_\infty=0.
$$

Taking the divergence gives $\nabla^2p_\infty=0$, and a further [Laplacian](../../../../laplacian.md) therefore gives

$$
\boxed{\nabla^4\mathbf u_\infty=\frac1\mu\nabla(\nabla^2p_\infty)=0.}
$$

Each [velocity](../../../../velocity.md) component obeys the [biharmonic equation](../../../../biharmonic-equation.md) in the whole ball.

Expand a component of $\mathbf u_\infty$ at the centre and average over $\mathbf x=a\mathbf n$. The odd spherical moments vanish, while

$$
\langle n_i n_j\rangle=\frac13\delta_{ij},\qquad
\langle n_i n_j n_k n_l\rangle
=\frac1{15}(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

Thus the [spherical mean of a biharmonic function](../../../../spherical-mean-of-a-biharmonic-function.md) gives

$$
\langle\mathbf u_\infty\rangle_{S_a}
=\left[1+\frac{a^2}{6}\nabla^2+\frac{a^4}{120}\nabla^4+\cdots\right]
\mathbf u_\infty(0)
=\mathbf u_\infty(0)+\frac{a^2}{6}\nabla^2\mathbf u_\infty(0).
$$

The truncation is exact, not just a small-sphere approximation: all terms containing two or more Laplacians vanish. One can avoid any Taylor-convergence issue by letting $M(r)=\langle\mathbf u_\infty(r\mathbf n)\rangle$. Since $\nabla^2\mathbf u_\infty$ is harmonic, its [spherical mean](../../../../spherical-mean.md) is $\nabla^2\mathbf u_\infty(0)$, so

$$
M''+\frac2rM'=\nabla^2\mathbf u_\infty(0),\qquad M(0)=\mathbf u_\infty(0),\quad M'(0)=0.
$$

Integrating gives $M(r)=\mathbf u_\infty(0)+r^2\nabla^2\mathbf u_\infty(0)/6$ for every admissible $r$.

Combining with the force-free result of part [c](../c.md) proves [Faxén's first law](../../../../faxen-s-first-law.md) in the requested form:

$$
\boxed{\mathbf V=\left.\left(1+\frac{a^2}{6}\nabla^2\right)\mathbf u_\infty\right|_{\mathbf x=0}.}
$$

The force-free qualification carries over. Local absence of ambient [body forces](../../../../body-force.md) and regularity inside the ball are also needed; if forcing or a singularity lies inside it, the harmonic-pressure and biharmonic-mean argument does not apply unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
