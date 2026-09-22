<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $a(y)=(1-y^2)^2$. Multiply $u_{xx}=\partial_y(au_y)$ by $2u_x$ and integrate over $-1<y<1$. An [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\frac d{dx}\int_{-1}^1u_x^2\,dy
&=2\bigl[au_xu_y\bigr]_{-1}^1-2\int_{-1}^1a u_{xy}u_y\,dy\\
&=-\frac d{dx}\int_{-1}^1a u_y^2\,dy,
\end{aligned}
$$

because $a(1)=a(-1)=0$. Therefore the [energy estimate](../../../../../../energy-estimate.md) is in fact the conservation law

$$
\boxed{\frac d{dx}\int_{-1}^1\left(u_x^2+(1-y^2)^2u_y^2\right)dy=0.}
$$

If $u(0,y)=u_x(0,y)=0$, then differentiating the first identity in $y$ also gives $u_y(0,y)=0$, so the conserved nonnegative energy is zero. Hence $u_x=0$ and $(1-y^2)u_y=0$ throughout the open strip. There $|y|<1$, so both derivatives vanish; connectedness and the initial value now give

$$
\boxed{u(x,y)=0\qquad((x,y)\in\mathbb R\times(-1,1)).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
