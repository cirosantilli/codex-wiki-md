<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Let $\mathbf e_r,\mathbf e_\phi,\mathbf e_z$ be the cylindrical unit vectors. The surface has an upward [normal vector](../../../../../normal-vector.md) proportional to $\mathbf e_z-h'(r)\mathbf e_r$. If $N_z$ is the vertical component of the [normal force](../../../../../normal-force.md), its radial component is $-h'(r)N_z$. In the stated approximation, vertical acceleration and the vertical driving-force component are neglected, so vertical balance gives $N_z\simeq Mg$. The horizontal contact [force](../../../../../force.md) is consequently $-Mg h'(r)\mathbf e_r$. The projected velocity and its speed are

$$
\mathbf v_h=\dot r\,\mathbf e_r+r\dot\phi\,\mathbf e_\phi,\qquad
u=\sqrt{\dot r^2+r^2\dot\phi^2}.
$$

The driving [force](../../../../../force.md) is parallel to this velocity, with components $F\dot r/u$ and $Fr\dot\phi/u$. Use the [acceleration in polar coordinates](../../../../../acceleration-in-polar-coordinates.md) and [Newton's second law](../../../../../newton-s-second-law.md) to obtain

$$
\boxed{\ddot r-r\dot\phi^2=-g h'(r)+\frac FM\frac{\dot r}{u},\qquad
r\ddot\phi+2\dot r\dot\phi=\frac FM\frac{r\dot\phi}{u}.}
$$

These equations apply where $u\ne0$; at rest the direction of an exactly velocity-aligned drive is not determined.

For a prescribed path, write $r'=dr/d\phi$, $r''=d^2r/d\phi^2$. The [chain rule](../../../../../chain-rule.md) gives $\dot r=r'\dot\phi$ and $\ddot r=r''\dot\phi^2+r'\ddot\phi$. Subtract $r'/r$ times the azimuthal equation from the radial equation. The driving [force](../../../../../force.md) and $\ddot\phi$ both cancel:

$$
\left(r''-r-\frac{2r'^2}{r}\right)\dot\phi^2=-g h'(r).
$$

Thus the constraint for [tangentially driven motion on an axisymmetric surface](../../../../../tangentially-driven-motion-on-an-axisymmetric-surface.md) is

$$
\boxed{\dot\phi^2=\frac{g h'(r)}{r+2r'^2/r-r''}.}
$$

The denominator must give a nonnegative squared speed, and the calculation uses $r>0$. At the polar origin a limiting Cartesian description is appropriate.

For the paraboloid and [Archimedean spiral](../../../../../archimedean-spiral.md), put

$$
\alpha=\sqrt{\frac{2g}{\ell}},\qquad
h'(r)=\frac{2r}{\ell},\qquad r=\epsilon\phi,\quad r'=\epsilon,\quad r''=0.
$$

Then, for $\phi>0$,

$$
\dot\phi^2=\alpha^2\frac{\phi^2}{\phi^2+2}.
$$

The branch tending to $\phi=\infty$ has positive [angular velocity](../../../../../angular-velocity.md), hence

$$
\dot\phi=\frac{\alpha\phi}{\sqrt{\phi^2+2}}\longrightarrow\alpha,\qquad
\ddot\phi=\frac{2\alpha^2\phi}{(\phi^2+2)^2}.
$$

Since $u=\epsilon\dot\phi\sqrt{1+\phi^2}$, solve the azimuthal equation for the required [force](../../../../../force.md):

$$
\frac FM=\epsilon\sqrt{1+\phi^2}
\left(\ddot\phi+\frac{2\dot\phi^2}{\phi}\right)
=\frac{2\epsilon\alpha^2\phi(\phi^2+3)\sqrt{\phi^2+1}}{(\phi^2+2)^2}.
$$

This is positive for $\phi>0$, consistent with a forward drive. Taking the limit gives

$$
\boxed{\dot\phi(t)\longrightarrow\sqrt{\frac{2g}{\ell}},\qquad
F(t)\longrightarrow\frac{4\epsilon Mg}{\ell}.}
$$

These are the large-time limits of the printed projected equations. Their mechanical approximation has a precise range limitation: on the exact surface, $z=h(r)$ gives $\dot z=(2r/\ell)\dot r$, which along this solution grows like $2\epsilon^2\alpha\phi/\ell$. At fixed positive $\epsilon$, it is not small as $\phi\to\infty$. Thus the requested limits are formal limits of that reduced model; neglect of vertical motion is not a uniform approximation to the full three-dimensional motion all the way to infinity.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
