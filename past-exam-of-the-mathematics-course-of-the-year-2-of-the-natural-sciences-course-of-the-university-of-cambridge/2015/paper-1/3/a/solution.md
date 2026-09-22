<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Green function](../../../../../green-s-function-split.md) of $D_x^2-1$, the homogeneous solutions satisfying the left and right endpoint conditions are $u(x)=\sinh x$ and $v(x)=\sinh(1-x)$. Their [Wronskian](../../../../../wronskian.md) is

$$
W=uv'-u'v=-\sinh1.
$$

Continuity of the kernel at $x=\xi$ and [integration](../../../../../integral-split.md) of $G_{xx}-G=\delta(x-\xi)$ require $[G_x]_{\xi-}^{\xi+}=1$. Hence the [Dirichlet modified Helmholtz Green function on an interval](../../../../../dirichlet-modified-helmholtz-green-function-on-an-interval.md) is

$$
\boxed{G(x,\xi)=-\frac{\sinh(x_<)\sinh(1-x_>)}{\sinh1}.}
$$

Here $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. The negative sign is essential for this operator convention. Integrating the forcing against the kernel gives

$$
\boxed{y(x)=-\frac1{\sinh1}\left[\sinh(1-x)\int_0^x\sinh\xi\,f(\xi)\,d\xi+\sinh x\int_x^1\sinh(1-\xi)f(\xi)\,d\xi\right].}
$$

This satisfies both endpoint conditions. It solves the equation classically for continuous $f$, and in the corresponding weak sense for integrable forcing. A homogeneous difference satisfying both endpoint conditions must vanish, so the solution is unique.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
