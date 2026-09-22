<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

For

$$
F(x,y,y')=y'^2+yy'+y'+y^2+yx^2,
$$

the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\frac d{dx}(2y'+y+1)-(y'+2y+x^2)=0,
$$

or

$$
y''-y=\frac{x^2}{2}.
$$

The general solution of this [inhomogeneous linear differential equation](../../../../../inhomogeneous-linear-differential-equation.md) is

$$
y(x)=Ce^x+De^{-x}-\frac{x^2}{2}-1.
$$

The condition $y(0)=-1$ gives $C+D=0$, and the condition at $x=1$ gives $C=1$. Therefore

$$
\boxed{y(x)=e^x-e^{-x}-\frac{x^2}{2}-1}.
$$

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
