<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [function](../../../../../../function-split.md) $y_1=x$ solves the [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation-split.md). Apply [reduction of order](../../../../../../reduction-of-order.md) by writing $y=xv(x)$. Substituting $y'=v+xv'$ and $y''=2v'+xv''$ and cancelling the terms in $v$ gives

$$
x^2(1-x)v''+(2x-3x^2)v'=0.
$$

For $w=v'$, this becomes a first-order [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation-split.md):

$$
w'+\left(\frac2x+\frac1{x-1}\right)w=0,\qquad w=\frac{C}{x^2(x-1)}.
$$

A [partial fraction decomposition](../../../../../../partial-fraction-decomposition.md) provides the required [antiderivative](../../../../../../antiderivative.md):

$$
\frac1{x^2(x-1)}=-\frac1x-\frac1{x^2}+\frac1{x-1},\qquad v=C_1+C_2\left(\log\frac{x-1}{x}+\frac1x\right).
$$

Therefore

$$
\boxed{y(x)=C_1x+C_2\left(1+x\log\frac{x-1}{x}\right),\qquad x>1.}
$$

The [logarithm](../../../../../../logarithm.md) has positive argument on the required [interval](../../../../../../interval-mathematics.md). The [Wronskian](../../../../../../wronskian.md) of $x$ and $1+x\log((x-1)/x)$ is $1/(x-1)\ne0$, proving their [linear independence](../../../../../../linear-independence.md) and hence completeness of this [general solution](../../../../../../general-solution.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
