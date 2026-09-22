<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

At a regular constrained stationary point of $F$ on $G=0$, the [Lagrange multiplier](../../../../../lagrange-multiplier.md) method solves

$$
\nabla F=\lambda\nabla G,
\qquad G=0.
$$

For the first problem, substitute $z=1+xy$ to obtain

$$
F=x^2+y^2+(1+xy)^2.
$$

Its stationary equations imply either $x=y$ or $xy=0$, and in either case the only real stationary point is $x=y=0$, $z=1$. Coercivity ensures that the minimum is attained, so

$$
\boxed{\min(x^2+y^2+z^2)=1}
$$

at $(0,0,1)$.

For the second problem, the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) gives

$$
-xy\leq\frac{x^2+y^2}{2}=\frac{1-z^2}{2}.
$$

Consequently

$$
z-xy\leq z+\frac{1-z^2}{2}
=1-\frac{(z-1)^2}{2}\leq1.
$$

Equality occurs at $(0,0,1)$, and hence

$$
\boxed{\max_{x^2+y^2+z^2=1}(z-xy)=1}.
$$

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
