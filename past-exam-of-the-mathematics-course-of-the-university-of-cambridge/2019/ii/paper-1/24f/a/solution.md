<h1 id="24f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
F(x,y)=x^3y+y^3+x.
$$

Its complex partial derivatives are

$$
F_x=3x^2y+1,
\qquad
F_y=x^3+3y^2.
$$

There is no point of $X'$ at which both vanish. Indeed, if $F=F_x=F_y=0$, then $F_y=0$ and $F=0$ give

$$
x^3=-3y^2,
\qquad
x=2y^3.
$$

Neither $x$ nor $y$ can be zero because $F_x=0$. Substitution into $F_x=0$ gives $12y^7+1=0$, whereas substitution into $F_y=0$ gives $8y^7+3=0$; these equations are incompatible.

For every $p=(x_0,y_0)\in X'$, at least one partial derivative is nonzero. If $F_y(p)\ne0$, the [holomorphic implicit function theorem](../../../../../../holomorphic-implicit-function-theorem.md) expresses the curve near $p$ as $y=g(x)$, and the restriction of the $x$-projection is a holomorphic coordinate chart. If $F_x(p)\ne0$, use the $y$-projection instead. On overlaps, the transition functions are restrictions of holomorphic coordinate functions and are holomorphic. These charts define an atlas making $X'$ a one-dimensional [complex manifold](../../../../../../complex-manifold.md), hence a [Riemann surface](../../../../../../riemann-surfaces.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24F](../../24f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
