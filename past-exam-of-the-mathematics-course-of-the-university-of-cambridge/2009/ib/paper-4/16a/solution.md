<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

Away from $x=\xi$, the [Dirichlet Green function](../../../../../dirichlet-green-function.md) solves the homogeneous equation. The endpoint conditions select $Ay_1(x)$ on the left and $By_2(x)$ on the right. Continuity and the unit derivative jump needed for a [Dirac delta function](../../../../../dirac-delta-function.md) give

$$
Ay_1(\xi)=By_2(\xi),\qquad
By_2'(\xi)-Ay_1'(\xi)=1.
$$

With [Wronskian](../../../../../wronskian.md) $W=y_1y_2'-y_1'y_2\ne0$, solve to obtain $A=y_2(\xi)/W(\xi)$ and $B=y_1(\xi)/W(\xi)$. Thus

$$
\boxed{G(x,\xi)=
\begin{cases}
y_1(x)y_2(\xi)/W(\xi),&x<\xi,\\
y_2(x)y_1(\xi)/W(\xi),&x>\xi.
\end{cases}}
$$

The first derivative term creates no extra delta because $G$ is continuous. The value at $x=\xi$ is the common limiting value.

For the specified constant-coefficient operator, take

$$
y_1(x)=e^{-x}-e^{-2x},\qquad
y_2(x)=e^{-x}-e^{1-2x},\qquad
W(\xi)=(e-1)e^{-3\xi}.
$$

Therefore its explicit [Green function](../../../../../green-s-function.md) is

$$
\boxed{G(x,\xi)=\frac{e^{3\xi}}{e-1}
\begin{cases}
(e^{-x}-e^{-2x})(e^{-\xi}-e^{1-2\xi}),&x<\xi,\\
(e^{-x}-e^{1-2x})(e^{-\xi}-e^{-2\xi}),&x>\xi.
\end{cases}}
$$

For the forcing step and the homogeneous endpoint conditions inherited from this Green-function problem, $y(x)=2\int_{x_0}^1G(x,\xi)\,d\xi$. When $x<x_0$, every integration point lies on the first branch, so

$$
\boxed{y(x)=\frac{2(e^{-x}-e^{-2x})}{e-1}\int_{x_0}^1(e^{2\xi}-e^{1+\xi})\,d\xi
=-\frac{(e-e^{x_0})^2}{e-1}(e^{-x}-e^{-2x}).}
$$

Without those endpoint conditions, an arbitrary homogeneous solution could also be added.

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
