<h1 id="18c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [curl](../../../../../../curl.md) of the linear momentum equation. For constant $\boldsymbol\Omega$ and zero [divergence](../../../../../../divergence.md), $\nabla\times(\boldsymbol\Omega\times\mathbf u)=-(\boldsymbol\Omega\cdot\nabla)\mathbf u$. With $\boldsymbol\Omega=\Omega\mathbf e_z$, this gives

$$
\partial_t\boldsymbol\omega=2\Omega\partial_z\mathbf u.
$$

Take another [curl](../../../../../../curl.md) and use part (a): $-\partial_t\nabla^2\mathbf u=2\Omega\partial_z\boldsymbol\omega$. Differentiate in time and substitute the previous equation:

$$
-\partial_t^2\nabla^2\mathbf u=4\Omega^2\partial_z^2\mathbf u.
$$

Consequently

$$
\boxed{\partial_t^2\nabla^2\mathbf u+4\Omega^2\partial_z^2\mathbf u=\mathbf0.}
$$

The two curl operations remove the pressure gradient while retaining the rotational restoring force.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18C](../../18c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
