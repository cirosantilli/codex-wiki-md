<h1 id="13c/solution">Solution</h1>

↑ **Parent:** [13C](../13c.md)

Write

$$
\mathbf u=\nabla\phi+\beta\nabla\alpha,
\qquad
\mathcal L=-\beta\alpha_t-\frac12\mathbf u\cdot\mathbf u.
$$

Variation of $\phi$ gives $\nabla\cdot\mathbf u=0$. Variation of $\alpha$ gives

$$
\beta_t+\nabla\cdot(\beta\mathbf u)=0,
$$

and variation of $\beta$ gives

$$
\alpha_t+\mathbf u\cdot\nabla\alpha=0.
$$

Using incompressibility, the middle equation becomes

$$
\beta_t+\mathbf u\cdot\nabla\beta=0.
$$

These are the three required Euler-Lagrange equations.

Let $D_t=\partial_t+\mathbf u\cdot\nabla$. Since $D_t\alpha=D_t\beta=0$, differentiating $u_i=\partial_i\phi+\beta\partial_i\alpha$ gives

$$
D_tu_i
=\partial_i(D_t\phi)-u_j\partial_i u_j
=\partial_i\left(D_t\phi-\frac12\mathbf u^2\right).
$$

Now

$$
D_t\phi
=\phi_t+\mathbf u\cdot\nabla\phi
=\phi_t+\mathbf u^2+\beta\alpha_t,
$$

because $\mathbf u\cdot\nabla\alpha=-\alpha_t$. Hence

$$
D_tu_i
=\partial_i\left(\phi_t+\beta\alpha_t+\frac12\mathbf u^2\right)
=-\partial_i p,
$$

where

$$
\boxed{p=-\frac12\mathbf u^2-\phi_t-\beta\alpha_t},
\qquad
\boxed{f(\phi_t,\alpha_t,\beta)=-\phi_t-\beta\alpha_t}.
$$

This is the [Clebsch-potential variational derivation of incompressible Euler flow](../../../../../clebsch-potential-variational-derivation-of-incompressible-euler-flow.md).

## ↑ Ancestors (10)

1. [13C](../13c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
