<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A returning orbit must have zero net change of the [energy](../../../../../../energy.md). To first order, integrate the perturbation along either unperturbed homoclinic loop:

$$
0=\int_{-\infty}^{\infty}(\beta-u_h^2)v_h^2\,d\tau
=\beta I_0-I_2.
$$

For the positive loop, $v_h=\pm u_h\sqrt{a_0^2-u_h^2/2}$; the outward and inward halves contribute equally. Therefore

$$
I_0=2\int_0^{\sqrt2a_0}u\sqrt{a_0^2-u^2/2}\,du=\frac43a_0^3,
$$

and

$$
I_2=2\int_0^{\sqrt2a_0}u^3\sqrt{a_0^2-u^2/2}\,du=\frac{16}{15}a_0^5.
$$

The [integrals](../../../../../../integral.md) follow by substituting $w=a_0^2-u^2/2$; for the second one use $u^2=2(a_0^2-w)$. Hence

$$
\boxed{\beta=\frac45a_0^2=-\frac45\alpha,\qquad
\kappa_{\rm hom}=-\frac45\lambda+o(|\lambda|),\quad\lambda<0.}
$$

The equality in rescaled parameters is the leading Melnikov balance, not an assertion that the entire finite-parameter [bifurcation](../../../../../../bifurcation.md) curve is exactly straight. Reflection [symmetry](../../../../../../symmetry-physics.md) makes both [saddle equilibrium](../../../../../../saddle-equilibrium.md) loops occur together. The global curve lies below the nonzero-equilibrium Hopf line $\kappa=-\lambda$, as shown in the parameter sketch.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
