<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

For a time-independent current, the [Maxwell equations](../../../../../maxwell-equations.md) reduce to [magnetostatics](../../../../../magnetostatics.md):

$$
\nabla\mathbin\cdot\mathbf B=0,
\qquad
\nabla\mathbin\times\mathbf B=\mu_0\mathbf j.
$$

Write $\mathbf B=\nabla\mathbin\times\mathbf A$ using a [vector potential](../../../../../vector-potential.md) and choose the [Coulomb gauge](../../../../../coulomb-gauge.md) $\nabla\mathbin\cdot\mathbf A=0$. The vector identity for the curl of a curl gives the [Poisson equation](../../../../../poisson-equation.md)

$$
-\nabla^2\mathbf A=\mu_0\mathbf j.
$$

The free-space [Green function](../../../../../green-s-function.md) therefore gives

$$
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int_V
\frac{\mathbf j(\mathbf r')}{|\mathbf r-\mathbf r'|}\,dV'.
$$

Taking the [curl](../../../../../curl.md) with respect to $\mathbf r$, moving it under the integral, and using $\nabla(1/|\mathbf r-\mathbf r'|)=-(\mathbf r-\mathbf r')/|\mathbf r-\mathbf r'|^3$ gives the [Biot-Savart law](../../../../../biot-savart-law.md)

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0}{4\pi}\int_V
\frac{\mathbf j(\mathbf r')\mathbin\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}\,dV'.}
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
