<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

First consider the usual local reduction with sufficiently smooth coefficients. The [hyperbolic partial differential equation](../../../hyperbolic-partial-differential-equation.md) has two distinct characteristic directions because $S^2-RT>0$. Choose independent local [characteristic coordinates](../../../characteristic-coordinate.md) $\xi,\eta$ whose gradients satisfy

$$
R\xi_x^2+2S\xi_x\xi_y+T\xi_y^2=0,\qquad
R\eta_x^2+2S\eta_x\eta_y+T\eta_y^2=0.
$$

Let $J=\xi_x\eta_y-\xi_y\eta_x\ne0$ and

$$
B=R\xi_x\eta_x+S(\xi_x\eta_y+\xi_y\eta_x)+T\xi_y\eta_y.
$$

The determinant of the transformed principal coefficient matrix gives $B^2=J^2(S^2-RT)>0$. By the [chain rule](../../../chain-rule.md), the left side of the original [partial differential equation](../../../partial-differential-equation-split.md) becomes

$$
2B\,u_{\xi\eta}+A_\xi u_\xi+A_\eta u_\eta,
\qquad A_\xi=R\xi_{xx}+2S\xi_{xy}+T\xi_{yy},
$$

with the analogous expression for $A_\eta$. The original first [derivatives](../../../derivative.md) are $z_x=u_\xi\xi_x+u_\eta\eta_x$ and $z_y=u_\xi\xi_y+u_\eta\eta_y$. Substitution and division by $2B$ yield the requested mixed-derivative canonical form. The construction is local, in a neighborhood where the two characteristic foliations give a [diffeomorphism](../../../diffeomorphism.md).

There is a regularity qualification in the printed hypotheses: merely continuous coefficients need not give twice continuously differentiable [characteristic coordinates](../../../characteristic-coordinate.md). Such coordinates are needed for the second-derivative [chain rule](../../../chain-rule.md) above. For example, take $R=0$, $S=1/2$ and $T=|x|$ near the origin. The characteristic equation factors as $\xi_y(\xi_x+|x|\xi_y)=0$. One family is $x=\text{constant}$ and the other has first integrals $\eta=h(y-x|x|/2)$. For an independent coordinate $h'\ne0$, but $\eta_{xx}$ has opposite one-sided limits at $x=0$. Hence no twice continuously differentiable characteristic coordinate system exists there. This illustrates that [continuous hyperbolic coefficients need not admit smooth characteristic coordinates](../../../continuous-hyperbolic-coefficients-need-not-admit-smooth-characteristic-coordinates.md). The formal general argument requires additional smoothness, for example twice continuously differentiable coefficients. The concrete coefficients below are smooth, so this issue does not affect their solution.

For the concrete [partial differential equation](../../../partial-differential-equation-split.md), put

$$
\xi=\frac{x}{y^2},\qquad\eta=y\quad(y>0).
$$

The [Jacobian determinant](../../../jacobian-determinant.md) is $1/y^2\ne0$. Direct use of the [chain rule](../../../chain-rule.md) gives

$$
z_{xx}=\frac{u_{\xi\xi}}{y^4},\qquad
z_{xy}=-\frac{2\xi u_{\xi\xi}}{y^3}+\frac{u_{\xi\eta}}{y^2}-\frac{2u_\xi}{y^3}.
$$

Therefore

$$
\boxed{u_{\xi\eta}=\frac2\eta u_\xi.}
$$

To impose the data efficiently, let $v=z_x$. Then $2xv_x+yv_y=0$, whose [characteristic curves](../../../characteristic-curve.md) preserve $x/y^2$, so $v=H(x/y^2)$. On the initial line $x=1$, the value $v(1,y)=y^2$ gives $H(\xi)=1/\xi$ for every $\xi>0$. Thus $z_x=y^2/x$, and integration in $x$ gives $z=y^2\log x+C(y)$. The remaining initial condition gives $C(y)=0$:

$$
\boxed{z(x,y)=y^2\log x,\qquad x>0,\ y>0.}
$$

Every point in this region is reached from the data by a characteristic with positive $x/y^2$. The line $x=0$ separates these characteristics from those with $x<0$, and the logarithmic divergence prevents a smooth extension of this solution through $x=0$. The original condition restricts us to $y>0$.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
