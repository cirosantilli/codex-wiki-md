<h1 id="9/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Solve the two algebraic [constraints](../../../../../../constraint-mechanics.md) for the squared coordinates:

$$
x^2=\frac{z^2+u^2}{3},\qquad y^2=\frac{z^2-2u^2}{3}.
$$

On any nonsingular real branch, [implicit differentiation](../../../../../../implicit-differentiation.md) at fixed $u$ gives $(\partial x/\partial z)_u=z/(3x)$ and $(\partial y/\partial z)_u=z/(3y)$. Differentiating $z^2=2x^2+y^2$ with the other original coordinate fixed gives $(\partial z/\partial x)_y=2x/z$ and $(\partial z/\partial y)_x=y/z$. Therefore

$$
\boxed{\left(\frac{\partial x}{\partial z}\right)_u\left(\frac{\partial z}{\partial x}\right)_y+\left(\frac{\partial y}{\partial z}\right)_u\left(\frac{\partial z}{\partial y}\right)_x=\frac z{3x}\frac{2x}z+\frac z{3y}\frac yz=\frac23+\frac13=1.}
$$

This is the [multivariable chain rule](../../../../../../multivariable-chain-rule.md) applied to $z(x(z,u),y(z,u))=z$. These formulas assume the relevant denominators are nonzero and the chosen variables are valid local coordinates.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
