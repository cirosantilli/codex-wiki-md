<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The [chain rule](../../../../../chain-rule.md) gives $\partial_x=\partial_\xi+\beta\partial_\eta$ and $\partial_y=\alpha\partial_\xi+\partial_\eta$. The coefficients of $u_{\xi\xi}$ and $u_{\eta\eta}$ are $2+3\alpha^2-7\alpha$ and $2\beta^2+3-7\beta$. Their integer roots are **$\alpha=2$ and $\beta=3$**. Thus choose [characteristic coordinates](../../../../../characteristic-coordinate.md) $\xi=x+2y$, $\eta=3x+y$, whose Jacobian determinant is $-5\ne0$. The coefficient of $u_{\xi\eta}$ is $4\beta+6\alpha-7(1+\alpha\beta)=-25$, so the equation becomes $-25u_{\xi\eta}=0$, equivalently $u_{\xi\eta}=0$.

Integrating the transformed [hyperbolic partial differential equation](../../../../../hyperbolic-partial-differential-equation.md) gives $u=F(\xi)+G(\eta)$. Along $x=-2y$ the coordinates are $(0,-5y)$, so the zero [boundary condition](../../../../../boundary-condition.md) gives $G(\eta)=-F(0)$ for every real $\eta$. Along $x=0$ they are $(2y,y)$, so $F(2y)-F(0)=4y^2$, hence $F(\xi)=\xi^2+F(0)$. The constants cancel and the unique resulting solution is

$$
\boxed{u(x,y)=(x+2y)^2.}
$$

It directly satisfies both [boundary conditions](../../../../../boundary-condition.md) and $2u_{xx}+3u_{yy}-7u_{xy}=4+24-28=0$.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
