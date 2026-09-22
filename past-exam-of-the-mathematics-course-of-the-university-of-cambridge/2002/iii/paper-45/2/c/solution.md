<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the growing density mode, write $\delta(\mathbf x,t)=b(t)\delta_*(\mathbf x)$. The new Poisson equation gives $\nabla_x^2\psi=\delta_*$ with no time dependence. With periodic zero-mean or fixed decaying boundary conditions, this determines a time-independent $\psi$ up to a spatially constant, dynamically irrelevant function. Thus

$$
\boxed{\partial_t\psi=0\quad\text{for the growing density mode, with fixed boundary conditions.}}
$$

In the linear continuity equation, $\partial_b\delta=\delta_*$, so $\nabla_x\cdot\mathbf u=-\delta_*=-\nabla_x^2\psi$. For the pure longitudinal growing mode, this gives $\mathbf u=-\nabla_x\psi$ and hence a time-independent scaled velocity. Equivalently, neglect the quadratic advection term in the motion equation and put $\mathbf h=\mathbf u+\nabla_x\psi$. It obeys

$$
\frac{d\mathbf h}{db}=-\frac{3\Omega}{2bf^2}\mathbf h,
\qquad \mathbf h(\mathbf x,t)=\frac{\mathbf C(\mathbf x)}{a^2\dot b}.
$$

The second expression follows directly from $\ddot b+2H\dot b=Cb/a^3$: its logarithmic derivative with respect to $b$ is the negative coefficient in the first equation. Excluding the homogeneous decaying-velocity component, $\mathbf C=0$, yields the [pure growing-mode scaled velocity](../../../../../../pure-growing-mode-scaled-velocity.md)

$$
\boxed{\partial_b\mathbf u=0,\qquad \partial_t\mathbf u=0.}
$$

The same holds along a trajectory to first order, since $\mathbf u\cdot\nabla\mathbf u$ is second order.

The pure growing-velocity assumption matters. A growing density alone does not exclude a divergence-free decaying velocity. For example, in an [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md) with $b=a$, one may add $\mathbf u_h=a^{-3/2}\sin(kx)\,\mathbf e_y$. Its divergence is zero, it solves the homogeneous linear motion equation, and it changes neither $\delta=b\delta_*$ nor $\psi$, yet it is not constant. Thus the printed constant-velocity statement is correct for the intended pure scalar growing mode; without that condition the displayed field is a counterexample. This extra mode is removed by the usual irrotational, no-decaying-mode initial conditions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
