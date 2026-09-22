<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

For a smooth [vector field](../../../../../vector-field.md) near an oriented piecewise smooth surface $S$, [Stokes theorem](../../../../../stokes-theorem.md) states

$$
\oint_{\partial S}\mathbf A\cdot d\mathbf x
=\int_S(\nabla\times\mathbf A)\cdot d\mathbf S,
$$

where the boundary orientation is induced by the surface [unit normal](../../../../../unit-normal.md) through the right-hand rule. For a constant vector $\mathbf k$, the [curl](../../../../../curl.md) of $\phi\mathbf k$ is $\nabla\phi\times\mathbf k$. Apply [Stokes theorem](../../../../../stokes-theorem.md) and use the scalar triple product:

$$
\mathbf k\cdot\oint_{\partial S}\phi\,d\mathbf x
=\int_S(\nabla\phi\times\mathbf k)\cdot d\mathbf S
=\mathbf k\cdot\int_Sd\mathbf S\times\nabla\phi.
$$

Since this holds for every constant $\mathbf k$, equality of all vector components proves the [vector-valued Stokes identity](../../../../../vector-valued-stokes-identity.md)

$$
\boxed{\int_Sd\mathbf S\times\nabla\phi=\oint_{\partial S}\phi\,d\mathbf x}.
$$

For the specified field, the two axis segments contribute zero because $x^2y^4$ vanishes on them. On the arc the direct [line integral](../../../../../line-integral.md) is

$$
I=\int_0^{\pi/2}\cos^2\theta\sin^4\theta(\cos\theta-\sin\theta)\,d\theta.
$$

Its two terms give

$$
\int_0^{\pi/2}\cos^3\theta\sin^4\theta\,d\theta
=\int_0^1u^4(1-u^2)\,du=\frac2{35},
$$

and

$$
\int_0^{\pi/2}\cos^2\theta\sin^5\theta\,d\theta
=\int_0^1u^2(1-u^2)^2\,du=\frac8{105}.
$$

Therefore

$$
\boxed{I=-\frac2{105}}.
$$

One can also check the orientation and sign by [Stokes theorem](../../../../../stokes-theorem.md). For the upward-oriented quarter disk, $(\nabla\times\mathbf A)_z=2xy^4-4x^2y^3$. Polar integration gives

$$
\int_0^1r^6dr\int_0^{\pi/2}(2\cos\theta\sin^4\theta-4\cos^2\theta\sin^3\theta)d\theta
=\frac17\left(\frac25-\frac8{15}\right)=-\frac2{105},
$$

consistent with the positively oriented boundary in the question.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
