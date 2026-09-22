<h1 id="36a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume that $\mathbf v$ is constant. Set

$$
\tau=t_{\rm ret},\qquad
n=\frac{\mathbf R}{R},\qquad
\beta=\frac{\mathbf v}{c},\qquad
\kappa=1-n\cdot\beta,\qquad
D=R-\beta\cdot\mathbf R=R\kappa.
$$

[Implicit differentiation](../../../../../../implicit-differentiation.md) of $t=\tau+R(\tau)/c$ gives

$$
\partial_t\tau=\frac1\kappa,
\qquad
\nabla\tau=-\frac{n}{c\kappa}.
$$

Since $d\mathbf R/d\tau=-\mathbf v$, direct differentiation of $D$ yields

$$
\partial_tD=\frac{c(\beta^2-n\cdot\beta)}{\kappa},
\qquad
\mathbf v\cdot\nabla D
=-\frac{c(\beta^2-n\cdot\beta)}{\kappa}.
$$

Therefore

$$
(\partial_t+\mathbf v\cdot\nabla)D=0.
$$

The [Liénard–Wiechert potentials](../../../../../../lienard-wiechert-potential.md) for uniform motion have $\phi=q/(4\pi\epsilon_0D)$ and $\mathbf A=\mathbf v\phi/c^2$. The preceding identity consequently implies

$$
\partial_t\phi+\mathbf v\cdot\nabla\phi=0.
$$

As $\mathbf v$ is constant,

$$
\boxed{
\frac1{c^2}\frac{\partial\phi}{\partial t}
+\nabla\cdot\mathbf A
=\frac1{c^2}
\left(\partial_t\phi+\mathbf v\cdot\nabla\phi\right)=0.}
$$

**Thus the explicit uniformly moving potentials satisfy the [Lorenz gauge](../../../../../../lorenz-gauge-condition.md).**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [36A](../../36a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
