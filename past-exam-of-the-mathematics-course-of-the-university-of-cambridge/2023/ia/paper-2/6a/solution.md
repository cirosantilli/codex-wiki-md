<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

The [parameter sensitivity equation](../../../../../parameter-sensitivity-equation.md) follows by differentiating with respect to $\mu$ and writing $u=y_\mu$:

$$
u_x=u+x+y^2+2\mu yu,
\qquad u(0,\mu)=0.
$$

At $\mu=0$, $y_x=y$, $y(0)=1$, so $y(x,0)=e^x$. Then

$$
u_x-u=x+e^{2x},\qquad u(0,0)=0,
$$

and the integrating factor $e^{-x}$ yields

$$
u(x,0)=e^{2x}-x-1.
$$

Equating powers in $y=y_0+\mu y_1+\mu^2y_2+\cdots$ gives

$$
y_0=e^x,\qquad y_1=e^{2x}-x-1,
$$



$$
y_2'-y_2=2y_0y_1,\qquad y_2(0)=0.
$$

Consequently

$$
\boxed{y_2=e^x(e^{2x}-1-x^2-2x).}
$$

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
