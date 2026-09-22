<h1 id="16a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $U(y)=c^2-y^2$, [completing the square](../../../../../../completing-the-square.md) gives the [Bogomolny bound](../../../../../../bogomolny-bound.md)

$$
\begin{aligned}
I[y]
&=\frac12\int_{-\infty}^{\infty}\left[(y'-U(y))^2+2U(y)y'\right]dx\\
&=\frac12\int_{-\infty}^{\infty}(y'-U(y))^2dx
+\int_{-c}^{c}(c^2-y^2)\,dy\\
&=\frac12\int_{-\infty}^{\infty}(y'-U(y))^2dx+\frac{4c^3}{3}.
\end{aligned}
$$

Consequently

$$
\boxed{I[y]\geq\frac{4c^3}{3}},
$$

with equality exactly when the [Bogomolny equation](../../../../../../bogomolny-equations.md)

$$
y'=c^2-y^2
$$

holds everywhere. Separating variables, or differentiating the proposed form directly, gives all solutions with the required limits:

$$
\boxed{y(x)=c\tanh\{c(x-x_0)\}},
\qquad x_0\in\mathbb R.
$$

These are the translated [phi-four kinks](../../../../../../phi-four-kink.md).

Differentiating the first-order equation yields

$$
y''=-2yy'=(-2y)(c^2-y^2)=U'(y)U(y),
$$

which is precisely the Euler-Lagrange equation from part (a). Thus every configuration saturating the first-order bound is automatically a stationary solution of the second-order variational equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16A](../../16a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
