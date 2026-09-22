<h1 id="8b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The only positive equilibrium solves $1-y=0$ and $x-1=0$, hence is

$$
\boxed{(x,y)=(1,1)}.
$$

Away from a nullcline,

$$
\frac{dy}{dx}
=\frac{3y(x-1)}{x(1-y)}.
$$

This is separable:

$$
\left(\frac1y-1\right)dy
=3\left(1-\frac1x\right)dx.
$$

Integration gives the [first integral](../../../../../../first-integral.md)

$$
\log y-y=3x-3\log x+C.
$$

Thus one convenient conserved quantity is

$$
\boxed{E(x,y)=3x-3\log x+y-\log y}.
$$

Its gradient is

$$
\nabla E=\left(3-\frac3x,\,1-\frac1y\right),
$$

so $(1,1)$ is its only stationary point in the positive quadrant. Its [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
\nabla^2E=
\begin{pmatrix}3/x^2&0\\0&1/y^2\end{pmatrix},
$$

which is positive definite everywhere. Hence $(1,1)$ is a strict, indeed global, minimum.

The nearby level curves of $E$ are closed curves surrounding this minimum. Since $E$ is constant along every trajectory, a solution starting on a sufficiently small nearby level set cannot leave the region bounded by a slightly larger level set. This proves [Lyapunov stability](../../../../../../lyapunov-stability.md) of the equilibrium: solutions initially close to $(1,1)$ remain close for all time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
