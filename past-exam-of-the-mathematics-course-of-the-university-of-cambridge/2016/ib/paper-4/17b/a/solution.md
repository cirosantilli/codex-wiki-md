<h1 id="17b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the positive logarithmic fundamental solution used here, a [Dirichlet Green function](../../../../../../dirichlet-green-function.md) for an interior pole $\mathbf r_0$ satisfies

$$
\nabla_{\mathbf r}^2G(\mathbf r,\mathbf r_0)=\delta(\mathbf r-\mathbf r_0),\qquad G=0\text{ on }\partial\mathcal D.
$$

Equivalently, $G-G_0$ is harmonic near the pole, $G$ is harmonic away from it, and it has the specified logarithmic singularity. Regularity up to the remaining boundary is understood; on an unbounded domain impose the appropriate condition at infinity as well.

Apply [Green second identity](../../../../../../green-second-identity.md) with $f=\psi$ and $g=G$. Since $\psi$ is a [harmonic function](../../../../../../harmonic-function.md), the volume integral is $\int\psi\delta_{\mathbf r_0}\,dA=\psi(\mathbf r_0)$. The term $G\partial_n\psi$ vanishes on the boundary by the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md). Therefore

$$
\boxed{\psi(\mathbf r_0)=\int_{\partial\mathcal D}\psi(\mathbf r)\,\partial_nG(\mathbf r,\mathbf r_0)\,dl.}
$$

One may equivalently excise a small disc around the pole and take its radius to zero. The sign is positive because this question uses $\nabla^2G=+\delta$, not the alternative negative-Laplacian convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
