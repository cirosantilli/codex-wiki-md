<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the divergence of the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md). Since the divergence of a curl is zero, [Gauss's law](../../../../../../gauss-s-law.md) gives

$$
0=\mu_0\nabla\cdot J
+\mu_0\epsilon_0\frac{\partial}{\partial t}(\nabla\cdot E)
=\mu_0\left(\nabla\cdot J+\frac{\partial\rho}{\partial t}\right).
$$

Thus

$$
\frac{\partial\rho}{\partial t}+\nabla\cdot J=0,
$$

which is [charge conservation from Maxwell equations](../../../../../../charge-conservation-from-maxwell-equations.md). Integrating over a fixed volume and using the divergence theorem yields

$$
\frac{dQ}{dt}=-\int_{\partial V}J\cdot n\,dS.
$$

Charge in $V$ is conserved provided no current crosses $\partial V$. For total charge in all space, the corresponding assumption is sufficient decay of $J$ so that the flux at infinity vanishes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
