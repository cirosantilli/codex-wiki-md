<h1 id="5c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After division by $x$, the coefficient of $y'$ is $P(x)=1/x-1$. The [Abel identity](../../../../../../abel-s-identity.md) for the [Wronskian](../../../../../../wronskian.md) gives

$$
W'=-P(x)W=\left(1-\frac1x\right)W,
$$

so

$$
\boxed{W(x)=C\frac{e^x}{x}}.
$$

For $\lambda=1$, direct substitution confirms that $y_1=1-x$. [Reduction of order](../../../../../../reduction-of-order.md) gives a second solution proportional to

$$
y_2=(1-x)\int\frac{e^x}{x(1-x)^2}\,dx.
$$

To extract the requested coefficients, put

$$
y_2=(1-x)\log x+b_1x+b_2x^2+\cdots.
$$

For the differential operator

$$
L[y]=xy''+(1-x)y'+y,
$$

one finds

$$
L[(1-x)\log x]=x-3.
$$

The analytic correction $h=\sum_{n\geq1}b_nx^n$ must therefore satisfy $L[h]=3-x$. Its constant and linear coefficients give

$$
b_1=3,\qquad 4b_2=-1.
$$

Hence

$$
\boxed{
y_2=(1-x)\log x+3x-\frac14x^2+\cdots}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5C](../../5c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
