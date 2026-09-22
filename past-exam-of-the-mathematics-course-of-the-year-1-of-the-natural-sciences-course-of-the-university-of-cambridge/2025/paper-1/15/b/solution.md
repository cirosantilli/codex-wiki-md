<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the given [differential form](../../../../../differential-form-split.md), set $P=x(y^4+1)$ and $Q=y(2x^2y^2+1)$. Their [partial derivatives](../../../../../partial-derivative.md) satisfy

$$
P_y=4xy^3=Q_x.
$$

In fact an explicit potential is

$$
F(x,y)=\frac12x^2(y^4+1)+\frac12y^2,
$$

since $F_x=P$ and $F_y=Q$. Thus the [differential form](../../../../../differential-form-split.md) is an [exact differential form](../../../../../exact-differential-form.md) on all of $\mathbb R^2$.

Replacing $y^2$ by $u$ suggests the potential

$$
H(x,u)=\frac12\left[x^2(u^2+1)+u\right].
$$

Direct [differentiation](../../../../../differentiation.md) verifies that $dH/dx$ is exactly the left-hand side of the required [ordinary differential equation](../../../../../ordinary-differential-equation.md). This direct verification remains valid even for negative $u$; it does not require a real square root $y=\sqrt u$. Therefore

$$
x^2u^2+u+x^2=C.
$$

The [initial condition](../../../../../initial-condition.md) gives $C=1$. Solving this [quadratic equation](../../../../../quadratic-equation.md) in $u$ and selecting the branch that has $u(1)=0$ gives

$$
\boxed{u(x)=\frac{-1+\sqrt{1+4x^2-4x^4}}{2x^2}=\frac{2(1-x^2)}{1+\sqrt{1+4x^2-4x^4}}.}
$$

The second expression also defines the removable value $u(0)=1$. The maximal open [interval](../../../../../interval-mathematics.md) containing $1$ on which this is a differentiable real solution is

$$
\boxed{-\sqrt{\frac{1+\sqrt2}{2}}<x<\sqrt{\frac{1+\sqrt2}{2}}.}
$$

At either endpoint the square root vanishes and $2x^2u+1=0$, while $x(u^2+1)\ne0$, so the original [ordinary differential equation](../../../../../ordinary-differential-equation.md) cannot hold there with a finite [derivative](../../../../../derivative.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
