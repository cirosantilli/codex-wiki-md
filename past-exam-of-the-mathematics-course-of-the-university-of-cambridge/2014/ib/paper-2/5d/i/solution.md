<h1 id="5d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the real [Fourier series](../../../../../../fourier-series-split.md) convention

$$
f(x)\sim \frac{a_0}{2}+\sum_{n\ge1}\bigl(a_n\cos(2\pi nx)+b_n\sin(2\pi nx)\bigr).
$$

The constant coefficient is $a_0=2\int_0^1x(1-x)\,dx=1/3$. Reflection about $x=1/2$ changes the sine factor's sign and preserves the quadratic, giving $b_n=0$. Two [integrations by parts](../../../../../../integration-by-parts.md), with $q=2\pi n$, give

$$
\int_0^1x(1-x)\cos(qx)\,dx=-\frac2{q^2},
\qquad a_n=-\frac1{\pi^2n^2}.
$$

Consequently the [Fourier series of a periodically extended quadratic arch](../../../../../../fourier-series-of-a-periodically-extended-quadratic-arch.md) is

$$
\boxed{f_{\rm per}(x)=\frac16-\frac1{\pi^2}\sum_{n=1}^\infty\frac{\cos(2\pi nx)}{n^2}.}
$$

The periodic function is continuous, including at integers where its value is zero. Its piecewise smoothness gives pointwise [Fourier series](../../../../../../fourier-series-split.md) convergence everywhere, and the summable coefficient bound gives uniform and absolute convergence.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5D](../../5d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
