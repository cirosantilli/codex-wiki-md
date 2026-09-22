<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h=\Delta x$ and set $u_0=u_{M+1}=0$. In the discrete [L2 norm](../../../../../../l2-norm.md) $\|u\|_h^2=h\sum_{m=1}^M|u_m|^2$, the [energy method](../../../../../../energy-method.md) gives

$$
\frac12\frac{d}{dt}\|u\|_h^2
=-\frac1h\sum_{m=0}^M|u_{m+1}-u_m|^2\leq0.
$$

To obtain this identity, shift the indices in the centered second-difference sum. The centered first-difference [matrix](../../../../../../matrix.md) is [skew-symmetric](../../../../../../skew-symmetric-matrix.md), so its contribution has zero real part even for complex grid values. The homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) remove the endpoint terms.

Therefore the semidiscretization is **stable for every real $\alpha$ and every positive $h$**, with the mesh-independent bound $\|u(t)\|_h\leq\|u(0)\|_h$. No restriction on $|\alpha|h$ is needed for this energy estimate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
