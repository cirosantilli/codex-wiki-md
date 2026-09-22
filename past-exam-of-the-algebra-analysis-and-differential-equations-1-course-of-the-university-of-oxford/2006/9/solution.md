<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

The [characteristic equation of a partial differential equation](../../../characteristic-equation-of-a-partial-differential-equation.md) for $u_{xx}+u_{xy}=0$ is $(dy)^2-dx\,dy=0$. Thus the two [characteristic curve](../../../characteristic-curve.md) families are $\boxed{y=\text{constant},\quad y-x=\text{constant}}$. Set $\xi=y$ and $\eta=y-x$. The [chain rule](../../../chain-rule.md) gives $\partial_x=-\partial_\eta$ and $\partial_y=\partial_\xi+\partial_\eta$, reducing the equation to

$$
\boxed{U_{\xi\eta}=0.}
$$

Integrating in the two independent characteristic coordinates gives $U=F(\xi)+G(\eta)$, or $u(x,y)=F(y)+G(y-x)$. At $x=0$, the value condition gives $F(y)+G(y)=0$, while the derivative condition gives $-G'(y)=e^y$. Hence $G(y)=-e^y+C$ and $F(y)=e^y-C$, so

$$
\boxed{u(x,y)=e^y-e^{y-x}.}
$$

Direct differentiation gives $u_x=e^{y-x}$, $u_{xx}=-e^{y-x}$ and $u_{xy}=e^{y-x}$, verifying both the equation and the two data. The additive constants cancel in $u$, so they do not create different solutions.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2006](../../2006-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
