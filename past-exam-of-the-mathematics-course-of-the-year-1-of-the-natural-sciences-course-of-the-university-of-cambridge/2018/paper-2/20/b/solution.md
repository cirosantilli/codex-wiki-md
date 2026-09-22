<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On a smooth implicit branch, put $Q=x+z^2$ and require $Q\ne0$. This is exactly the [implicit function theorem](../../../../../implicit-function-theorem.md) condition, since the defining equation has vertical [partial derivative](../../../../../partial-derivative.md) $3Q$. Differentiating the cubic relation in $x$ and $y$ gives

$$
Qz_x=-z,\qquad Qz_y=1,
\qquad z_x=-\frac zQ,\quad z_y=\frac1Q.
$$

For a second [derivative](../../../../../derivative.md), the dependence of $Q$ on $z$ must also be included: $Q_x=1+2zz_x$ and $Q_y=2zz_y$. Thus

$$
\begin{aligned}
z_{xx}&=-\frac{z_x}{Q}+\frac{z(1+2zz_x)}{Q^2}=\frac{2xz}{Q^3},\\
z_{yy}&=-\frac{2zz_y}{Q^2}=-\frac{2z}{Q^3},\\
z_{xy}&=-\frac{z_y}{Q}+\frac{2z^2z_y}{Q^2}=\frac{z^2-x}{Q^3}.
\end{aligned}
$$

The required cancellation follows immediately:

$$
\boxed{z_{xx}+xz_{yy}=\frac{2xz}{(x+z^2)^3}-\frac{2xz}{(x+z^2)^3}=0.}
$$

The verification is local to smooth branches with $x+z^2\ne0$; the implicit relation does not guarantee a differentiable function at its singular points.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
