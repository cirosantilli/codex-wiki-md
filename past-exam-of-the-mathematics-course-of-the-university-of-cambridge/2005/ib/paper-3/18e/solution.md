<h1 id="18e/solution">Solution</h1>

↑ **Parent:** [18E](../18e.md)

Differentiate the [velocity potential](../../../../../velocity-potential.md) in polar coordinates:

$$
\boxed{u_r=U(1-a^2/r^2)\cos\theta,\qquad u_\theta=-U(1+a^2/r^2)\sin\theta+\frac\kappa{2\pi r}}.
$$

At $r=a$ the normal velocity is zero. At large radius these components tend to $U\cos\theta,-U\sin\theta$, the polar components of uniform flow in the positive $x$ direction. The circulation around any concentric circle is $\int_0^{2\pi}u_\theta r\,d\theta=\kappa$. Although the potential's circulation term is multivalued, its velocity is single-valued and irrotational away from the excluded axis.

For steady inviscid constant-density flow, [Bernoulli equation](../../../../../bernoulli-equation.md) gives $p+\rho|u|^2/2=p_\infty+\rho U^2/2$. On the cylinder, $u_\theta=-2U\sin\theta+\kappa/(2\pi a)$, so

$$
\boxed{p(a,\theta)=p_\infty+\frac\rho2\left[U^2-\left(-2U\sin\theta+\frac\kappa{2\pi a}\right)^2\right]}.
$$

In the displayed force integral, every constant or $\sin^2\theta$ term has zero cosine and sine first moments. The cross term in pressure is $\rho U\kappa\sin\theta/(\pi a)$. Therefore, using exactly the positive-sign convention printed,

$$
\boxed{F_x=0,\qquad F_y=\rho U\kappa}
$$

per unit axial length, since $\int_0^{2\pi}\sin^2\theta\,d\theta=\pi$.

With the usual normal directed outward from the cylinder into the fluid, pressure exerts traction $-pn$, so the physical force of the fluid on the cylinder is instead $\boxed{(0,-\rho U\kappa)}$. The positive integral printed in the question has the opposite sign. This makes the convention explicit and is consistent with the [Kutta–Joukowski theorem](../../../../../kutta-joukowski-theorem.md) for positive counterclockwise circulation.

## ↑ Ancestors (10)

1. [18E](../18e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
