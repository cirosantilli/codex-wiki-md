<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

Work first on $x>0$, where the proposed [logarithm](../../../../../logarithm.md) is defined. Substitution of $y=x^m$ into the [Cauchy-Euler differential equation](../../../../../cauchy-euler-equation.md) gives the [indicial equation](../../../../../indicial-equation.md)

$$
m(m-1)+m+1=m^2+1=0.
$$

Its distinct [indicial roots](../../../../../indicial-root.md) are $m=\pm i$. Using $x^{\pm i}=e^{\pm i\log x}$ and [Euler's formula](../../../../../euler-s-formula.md), a real [basis](../../../../../basis.md) of solutions is $\cos(\log x),\sin(\log x)$. Their [Wronskian](../../../../../wronskian.md) is $1/x$, so they are [linearly independent](../../../../../linear-independence.md) and span the two-dimensional [solution space of a homogeneous linear differential equation](../../../../../solution-space-of-a-homogeneous-linear-differential-equation.md). Therefore

$$
\boxed{y(x)=A\cos(\log x)+B\sin(\log x),\qquad x>0.}
$$

For the requested [change of variables](../../../../../change-of-variables-formula.md), set $Y(z)=y(e^z)$. The [chain rule](../../../../../chain-rule.md) gives

$$
y'=\frac{Y'}x,\qquad y''=\frac{Y''-Y'}{x^2}.
$$

The transformed [second-order linear differential equation](../../../../../second-order-linear-differential-equation.md) is $Y''+Y=0$. Its [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are again $\pm i$, giving $Y(z)=A\cos z+B\sin z$. Substituting $z=\log x$ recovers precisely the previous [general solution](../../../../../general-solution.md).

If solutions on $x<0$ are wanted, the same calculation uses $z=\log|x|$ and gives independent constants on that interval. Zero is a [singular point of a differential equation](../../../../../singular-point-of-a-differential-equation.md); the logarithmic oscillations do not define a nonzero continuous solution through it.

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
