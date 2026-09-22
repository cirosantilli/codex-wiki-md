<h1 id="9b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Stokes theorem](../../../../../../stokes-theorem.md) gives

$$
I=\oint_{\partial S}\mathbf A\mathbin\cdot d\mathbf r.
$$

For the upward orientation, the outer circle $r=2,z=1$ is counterclockwise from above and the inner circle $r=1,z=4$ is clockwise. On a counterclockwise circle of radius $R$ and height $z$,

$$
\oint\mathbf A\mathbin\cdot d\mathbf r
=-R^2\int_0^{2\pi}(3\sin^2\theta+z\cos^2\theta)\,d\theta
=-\pi R^2(3+z).
$$

The outer circle contributes $-16\pi$. The inner circle would contribute $-7\pi$ counterclockwise and hence contributes $+7\pi$ with its induced clockwise orientation. Thus

$$
\boxed{I=-16\pi+7\pi=-9\pi},
$$

agreeing with the direct calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9B](../../9b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
