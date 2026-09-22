<h1 id="h/h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

For symmetric quadratic coefficient matrices, the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) give $T\ddot q+Vq=0$, where $T$ is the positive-definite [mass matrix](../../../../mass-matrix.md). Substitute a normal-mode oscillation $q=v\cos(\omega t+\phi)$ to get

$$
\boxed{(V-\omega^2T)v=0,\qquad\det(V-\omega^2T)=0.}
$$

The positive roots $\omega^2$ determine the squared normal frequencies and their nonzero null vectors give mode shapes. Repeated eigenvalues give multidimensional mode spaces.

The particle's [kinetic energy](../../../../kinetic-energy.md) is $m|\dot q|^2/2$. For a taut elastic string at length $r=\sqrt{x^2+y^2+z^2}$, [Hooke's law](../../../../hooke-s-law.md) gives tension $\lambda(r-a)/a$ and elastic energy $\lambda(r-a)^2/(2a)$. With $\lambda=mg$ and gravitational potential $mgz$, this gives exactly

$$
T=\frac m2(\dot x^2+\dot y^2+\dot z^2),\qquad
V=mgz+\frac{mg}{2a}(r-a)^2.
$$

This is the taut-string regime containing the equilibrium. Differentiating the potential gives

$$
\boxed{\ddot x=-\frac ga\frac{r-a}{r}x,\quad
\ddot y=-\frac ga\frac{r-a}{r}y,\quad
\ddot z=-g-\frac ga\frac{r-a}{r}z.}
$$

At $(0,0,-2a)$, $r=2a$ and all three accelerations vanish.

With $z=-2a+\zeta$, expansion to quadratic order gives $r=2a-\zeta+(x^2+y^2)/(4a)+O(3)$. Substitution cancels the linear terms, leaving

$$
\boxed{V=-\frac32mga+\frac{mg}{4a}(x^2+y^2)+\frac{mg}{2a}\zeta^2+O(3).}
$$

The [mass matrix](../../../../mass-matrix.md) remains $mI$, and the [stiffness matrix](../../../../stiffness-matrix.md) is $\operatorname{diag}(mg/(2a),mg/(2a),mg/a)$. Therefore

$$
\boxed{\omega_x=\omega_y=\sqrt{\frac g{2a}},\qquad
\omega_z=\sqrt{\frac ga}.}
$$

The horizontal frequency is doubly degenerate: a linearly polarized oscillation in any horizontal direction is a [normal mode](../../../../normal-mode.md). The remaining mode is vertical stretching and contraction of the string, with horizontal coordinates zero.

## ↑ Ancestors (12)

1. [H2](../h2.md)
2. [H](../../h.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
