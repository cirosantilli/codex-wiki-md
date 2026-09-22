<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

The homogeneous [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $r^2-r-2=(r-2)(r+1)=0$, so its solutions are $e^{2x}$ and $e^{-x}$. Because the forcing contains the latter exponential, set $y=e^{-x}v$. Direct differentiation reduces the [inhomogeneous linear differential equation](../../../../../inhomogeneous-linear-differential-equation.md) to

$$
v''-3v'=18x.
$$

A polynomial particular solution is $v=-3x^2-2x$, since $v''-3v'=-6-3(-6x-2)=18x$. Therefore

$$
y=C_1e^{2x}+e^{-x}(C_2-2x-3x^2).
$$

The exponentially growing first term cannot be canceled by the decaying second term, so boundedness at positive infinity requires $C_1=0$. The [initial condition](../../../../../initial-condition.md) $y(0)=1$ sets $C_2=1$. Hence

$$
\boxed{y(x)=(1-2x-3x^2)e^{-x}.}
$$

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
