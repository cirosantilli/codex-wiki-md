<h1 id="14a/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Transform in time and use the zero interior [initial conditions](../../../../../../../initial-condition.md). The [Laplace transform of a derivative](../../../../../../../laplace-transform-of-a-derivative.md) formula turns the [wave equation](../../../../../../../wave-equation-split.md) into $c^2Y_{xx}=p^2Y$. Its transformed endpoint conditions are $Y(0,p)=a/p$ and $Y(L,p)=0$. A [homogeneous solution](../../../../../../../homogeneous-solution.md) satisfying the right condition is a multiple of $\sinh[p(L-x)/c]$; the left condition fixes that multiple. Thus, for $\operatorname{Re}p>0$,

$$
\boxed{Y(x,p)=\frac{a\sinh[p(L-x)/c]}{p\sinh(pL/c)}.}
$$

Here $L,c>0$ and the denominator has no zeros in this half-plane. The initial-boundary corner at $(0,0)$ is deliberately discontinuous: the applied step launches propagating fronts, so one should not demand a globally smooth solution across them.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [14A](../../../14a.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
