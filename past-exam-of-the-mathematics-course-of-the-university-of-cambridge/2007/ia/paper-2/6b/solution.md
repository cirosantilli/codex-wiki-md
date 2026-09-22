<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Write $u(x,y)=U(\xi,\eta)$. The [chain rule](../../../../../chain-rule.md) gives $\partial_x=\partial_\xi+\partial_\eta$ and $\partial_y=2\partial_\xi+3\partial_\eta$. Consequently the coefficients of $U_{\xi\xi}$ and $U_{\eta\eta}$ cancel, while that of $U_{\xi\eta}$ is $12-25+12=-1$. The transformed [partial differential equation](../../../../../partial-differential-equation-split.md) is $-U_{\xi\eta}=1$. Integrating once in each variable gives the most general twice differentiable solution,

$$
\boxed{u(x,y)=-(x+2y)(x+3y)+F(x+2y)+G(x+3y),}
$$

where $F,G$ are arbitrary twice differentiable functions. The [change of variables](../../../../../change-of-variables-formula.md) is invertible because its [Jacobian determinant](../../../../../jacobian-determinant.md) is $3-2=1$.

On $y=0$, the value condition gives $F(x)+G(x)=x^2$. Differentiating it yields $F'(x)+G'(x)=2x$. The derivative condition gives $-5x+2F'(x)+3G'(x)=x$. Subtraction therefore gives $G'(x)=2x$ and $F'(x)=0$. The constants in $F$ and $G$ cancel in their sum, leaving

$$
\boxed{u(x,y)=(x+3y)^2-(x+2y)(x+3y)=xy+3y^2.}
$$

Indeed $u_{xx}=0$, $u_{xy}=1$, $u_{yy}=6$, so the original operator gives $-5+6=1$, and the two initial-line conditions hold.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
