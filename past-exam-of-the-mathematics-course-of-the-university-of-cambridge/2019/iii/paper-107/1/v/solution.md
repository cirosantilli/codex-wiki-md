<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Fix $x\in\Omega'$ and $0<\rho<R(\Omega')$. Differentiate the ball mean-value formula and apply the [divergence theorem](../../../../../../divergence-theorem.md):

$$
\partial_{x_j}u(x)
=\frac1{\omega_d\rho^d}\int_{B(x,\rho)}\partial_j u
=\frac1{\omega_d\rho^d}\int_{\partial B(x,\rho)}u\nu_j\,dS.
$$

Since $|\nu_j|\leq1$ and $|\partial B(x,\rho)|=d\omega_d\rho^{d-1}$,

$$
|\partial_{x_j}u(x)|\leq\frac d\rho\max_\Omega|u|.
$$

Letting $\rho\uparrow R(\Omega')$ and taking both maxima proves

$$
\boxed{\max_{1\leq j\leq d}\max_{\Omega'}|\partial_{x_j}u|\leq\frac d{R(\Omega')}\max_\Omega|u|.}
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
