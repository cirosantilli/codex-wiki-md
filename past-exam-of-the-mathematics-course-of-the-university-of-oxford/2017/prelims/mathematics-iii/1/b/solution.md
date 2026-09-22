<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $y=x$, the [derivatives](../../../../../../derivative.md) are $y'=1$ and $y''=0$, and substitution gives $2(x-1)-2(x-1)=0$.

Use [reduction of order](../../../../../../reduction-of-order.md): set $y=xv$, so $y'=v+xv'$ and $y''=2v'+xv''$. Substitution and cancellation give

$$
x^2v''+2x^2v'=0.
$$

Since $x>0$, this reduces to $v''+2v'=0$, hence $v'=Ae^{-2x}$ and $v=C_1+C_2e^{-2x}$. The [general solution](../../../../../../general-solution.md) is

$$
\boxed{y(x)=C_1x+C_2xe^{-2x},\qquad x>0.}
$$

The two solutions are [linearly independent](../../../../../../linear-independence.md), since their ratio $e^{-2x}$ is nonconstant; equivalently, their [Wronskian](../../../../../../wronskian.md) is $-2x^2e^{-2x}\ne0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
