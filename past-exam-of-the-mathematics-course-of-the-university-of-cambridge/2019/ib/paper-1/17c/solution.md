<h1 id="17c/solution">Solution</h1>

↑ **Parent:** [17C](../17c.md)

For an [incompressible flow](../../../../../incompressible-flow.md), $\nabla\cdot\mathbf u=0$. If the flow is also irrotational, then locally $\mathbf u=\nabla\phi$ for a [velocity potential](../../../../../velocity-potential.md), and therefore

$$
\nabla^2\phi=\nabla\cdot\mathbf u=0.
$$

The boundary conditions are

$$
\left.\frac{\partial\phi}{\partial r}\right|_{r=a}=0,
\qquad
\nabla\phi\longrightarrow U\mathbf e_x\quad(r\to\infty),
\qquad
\int_0^{2\pi}\frac{\partial\phi}{\partial\theta}\,d\theta=\kappa.
$$

The fluid region is not simply connected, so a potential may change by the constant $\kappa$ after one circuit while its gradient remains single-valued. Superposing uniform flow, the cylinder doublet, and the circulation gives the [potential flow around a circular cylinder with circulation](../../../../../potential-flow-around-a-circular-cylinder-with-circulation.md)

$$
\boxed{\phi(r,\theta)=U\left(r+\frac{a^2}{r}\right)\cos\theta+\frac\kappa{2\pi}\theta}.
$$

Its velocity components are

$$
u_r=U\left(1-\frac{a^2}{r^2}\right)\cos\theta,
\qquad
u_\theta=-U\left(1+\frac{a^2}{r^2}\right)\sin\theta+\frac\kappa{2\pi r}.
$$

On $r=a$, $u_r=0$ and, with $\lambda=\kappa/(4\pi Ua)$,

$$
u_\theta=2U(\lambda-\sin\theta).
$$

The [Bernoulli equation](../../../../../bernoulli-equation.md) gives $p=p_\infty+\rho(U^2-u_\theta^2)/2$. The pressure force per unit length on the cylinder is

$$
\mathbf F=-a\int_0^{2\pi}p\,\mathbf e_r\,d\theta
=\frac{\rho a}{2}\int_0^{2\pi}u_\theta^2(\cos\theta\,\mathbf e_x+\sin\theta\,\mathbf e_y)\,d\theta.
$$

The $x$ component vanishes by symmetry, while $\int_0^{2\pi}\sin^2\theta\,d\theta=\pi$ gives

$$
\boxed{\mathbf F=-4\pi\rho aU^2\lambda\,\mathbf e_y=-\rho\kappa U\,\mathbf e_y},
$$

in agreement with the [Kutta–Joukowski theorem](../../../../../kutta-joukowski-theorem.md).

A [stagnation point](../../../../../stagnation-point.md) satisfies $u_r=u_\theta=0$. On the cylinder this means $\sin\theta=\lambda$. Thus $|\lambda|<1$ gives two surface stagnation points, $|\lambda|=1$ gives one coincident surface point, and $|\lambda|>1$ gives none on the surface. Away from the cylinder, $u_r=0$ requires $\cos\theta=0$. Solving $u_\theta=0$ then gives one physical exterior root when $|\lambda|>1$:

$$
\boxed{r=a\left(|\lambda|+\sqrt{\lambda^2-1}\right),
\qquad
\theta=\begin{cases}\pi/2,&\lambda>1,\\3\pi/2,&\lambda<-1.
\end{cases}}
$$

At $|\lambda|=1$ this root lies on $r=a$ and agrees with the single surface point.

## ↑ Ancestors (10)

1. [17C](../17c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
