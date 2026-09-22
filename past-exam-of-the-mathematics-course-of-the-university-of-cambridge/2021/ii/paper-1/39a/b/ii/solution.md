<h1 id="39a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Both candidate fields are divergence-free. For solid-body rotation,

$$
\mathbf u=\boldsymbol\Omega\times\mathbf x,
$$

each component is linear in $\mathbf x$, so $\nabla^2\mathbf u=0$. Also,

$$
\mathbf u=\boldsymbol\Omega\times\nabla\left(\frac1r\right)
$$

is harmonic for $r>0$, because $\nabla^2(1/r)=0$ there and constant-coefficient derivatives commute with the Laplacian. Thus both solve the Stokes equations with $p=0$.

The rotationally symmetric solution is consequently

$$
\mathbf u
=\left(A+\frac B{r^3}\right)
\boldsymbol\Omega\times\mathbf x.
$$

The [no-slip boundary condition](../../../../../../../no-slip-boundary-condition.md) gives

$$
A+\frac B{a^3}=1,
\qquad
A+\frac B{b^3}=0.
$$

Therefore

$$
A=-\frac{a^3}{b^3-a^3},
\qquad
B=\frac{a^3b^3}{b^3-a^3},
$$

and

$$
\boxed{
\mathbf u(\mathbf x)
=\frac{a^3}{b^3-a^3}
\left(\frac{b^3}{r^3}-1\right)
\boldsymbol\Omega\times\mathbf x}.
$$

This is the [Rotational Stokes flow between concentric spheres](../../../../../../../rotational-stokes-flow-between-concentric-spheres.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [39A](../../../39a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
