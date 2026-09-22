<h1 id="36d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\boldsymbol\sigma$ be the stated [Maxwell stress tensor](../../../../../../maxwell-stress-tensor.md). Taking its divergence and using

$$
(\mathbf A\mathbin\cdot\nabla)\mathbf A
-\frac12\nabla|\mathbf A|^2
=-\mathbf A\times(\nabla\times\mathbf A)
$$

gives

$$
\begin{aligned}
\partial_j\sigma_{ij}
={}&\epsilon_0[\mathbf E\times(\nabla\times\mathbf E)]_i
-\epsilon_0E_i\nabla\mathbin\cdot\mathbf E\\
&+\frac1{\mu_0}[\mathbf B\times(\nabla\times\mathbf B)]_i
-\frac1{\mu_0}B_i\nabla\mathbin\cdot\mathbf B.
\end{aligned}
$$

The [Maxwell equations](../../../../../../maxwell-equations.md) in vacuum with sources are

$$
\nabla\mathbin\cdot\mathbf E=\frac\rho{\epsilon_0},
\qquad
\nabla\mathbin\cdot\mathbf B=0,
\qquad
\nabla\times\mathbf E=-\partial_t\mathbf B,
\qquad
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
$$

Substitution, together with antisymmetry of the [cross product](../../../../../../cross-product.md), yields

$$
\begin{aligned}
\partial_j\sigma_{ij}
&=-\rho E_i-(\mathbf J\times\mathbf B)_i
-\epsilon_0[\mathbf E\times\partial_t\mathbf B
+\partial_t\mathbf E\times\mathbf B]_i\\
&=-[\rho\mathbf E+\mathbf J\times\mathbf B]_i
-\partial_t[\epsilon_0\mathbf E\times\mathbf B]_i.
\end{aligned}
$$

Therefore the required vector is the [electromagnetic momentum density](../../../../../../electromagnetic-momentum-density.md)

$$
\boxed{\mathbf g=\epsilon_0\mathbf E\times\mathbf B
=\frac{\mathbf S}{c^2}},
$$

and

$$
\boxed{\sum_{j=1}^3\frac{\partial\sigma_{ij}}{\partial x_j}
+\frac{\partial g_i}{\partial t}
=-(\rho\mathbf E+\mathbf J\times\mathbf B)_i}.
$$

This is [local conservation of electromagnetic momentum](../../../../../../local-conservation-of-electromagnetic-momentum.md). The tensor component $\sigma_{ij}$ is the flux of $i$-momentum in the $j$ direction in the convention of the question, $\mathbf g$ is field momentum per unit volume, and $\rho\mathbf E+\mathbf J\times\mathbf B$ is the [Lorentz force density](../../../../../../lorentz-force-density.md) transferred to matter.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [36D](../../36d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
