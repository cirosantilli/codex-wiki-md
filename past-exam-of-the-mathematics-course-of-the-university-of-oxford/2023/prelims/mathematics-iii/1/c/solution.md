<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $y=x$, the first and second [derivatives](../../../../../../derivative.md) are one and zero, giving $-2x+2x=0$. To find an independent solution, use [reduction of order](../../../../../../reduction-of-order.md) and write $y=xv(x)$. Cancellation of the terms proportional to $v$ leaves

$$
x(1-x^2)v''+(2-4x^2)v'=0.
$$

Writing $w=v'$ and using [separation of variables](../../../../../../separation-of-variables.md) gives

$$
\frac{w'}w=-\frac2x+\frac{2x}{1-x^2},\qquad
w=\frac C{x^2(1-x^2)}.
$$

Since $1/[x^2(1-x^2)]=x^{-2}+(1-x^2)^{-1}$, integration yields the [general solution](../../../../../../general-solution.md)

$$
\boxed{y(x)=C_1x+C_2\left(\frac x2\log\frac{1+x}{1-x}-1\right),\qquad0<x<1.}
$$

The second factor divided by $x$ has nonzero [derivative](../../../../../../derivative.md) $1/[x^2(1-x^2)]$, so the two solutions are [linearly independent](../../../../../../linear-independence.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
