<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taking the Laplace transform in $t$ gives

$$
U_{xx}-sU=-f(x).
$$

The bounded resolvent solution supplied in the hint can be written

$$
U(x,s)=\int_{-\infty}^{\infty}\frac{e^{-\sqrt s|x-\xi|}}{2\sqrt s}f(\xi)\,d\xi.
$$

Part (a) inverts the kernel, yielding the [heat kernel](../../../../../../heat-kernel.md)

$$
\boxed{K(|x-\xi|,t)=\frac1{\sqrt{4\pi t}}\exp\left(-\frac{(x-\xi)^2}{4t}\right).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
