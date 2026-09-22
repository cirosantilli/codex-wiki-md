<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

The free-space [Green function of the Laplacian](../../../../../green-function-of-the-laplacian.md) for the [Poisson equation](../../../../../poisson-equation.md) gives the [electric potential](../../../../../electric-potential.md)

$$
\boxed{\phi(\mathbf x)=\frac1{4\pi\epsilon_0}
\int_{\mathbb R^3}\frac{\rho(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x'}.
$$

For $r=|\mathbf x|\gg R$, its [electric multipole expansion](../../../../../electric-multipole-expansion.md) begins with

$$
\frac1{|\mathbf x-\mathbf x'|}
=\frac1r+\frac{\widehat{\mathbf x}\cdot\mathbf x'}{r^2}+O(r^{-3}).
$$

Define the [total electric charge](../../../../../electric-charge.md) and [electric dipole moment](../../../../../electric-dipole-moment.md) by

$$
Q=\int\rho(\mathbf x')\,d^3x',
\qquad
\mathbf p=\int\mathbf x'\rho(\mathbf x')\,d^3x'.
$$

Then

$$
\boxed{\phi(\mathbf x)=\frac1{4\pi\epsilon_0}
\left(\frac Qr+\frac{\mathbf p\cdot\widehat{\mathbf x}}{r^2}+O(r^{-3})\right)}.
$$

The analogous solution for the [magnetic vector potential](../../../../../magnetic-vector-potential.md) is

$$
\boxed{\mathbf A(\mathbf x)=\frac{\mu_0}{4\pi}
\int_{\mathbb R^3}\frac{\mathbf J(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x'}.
$$

Its apparent $r^{-1}$ coefficient is $\mu_0(4\pi)^{-1}\int\mathbf J\,d^3x'$. For each component, the supplied identity and the [divergence-free vector field](../../../../../divergence-free-vector-field.md) condition give

$$
\int J_i\,d^3x'
=\int\frac{\partial}{\partial x'_j}(x'_iJ_j)\,d^3x'.
$$

The [divergence theorem](../../../../../divergence-theorem.md) turns this into a surface integral outside the compact support of the [current density](../../../../../current-density.md), where $\mathbf J=0$. Hence $\int\mathbf J\,d^3x'=0$, so the $1/r$ term vanishes.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
