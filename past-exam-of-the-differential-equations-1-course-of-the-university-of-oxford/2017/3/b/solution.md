<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In $x,y>0$, the [characteristic equation of a partial differential equation](../../../../characteristic-equation-of-a-partial-differential-equation.md) gives $dx/\sqrt x=\pm\sqrt y\,dy$. Integration yields the [characteristic coordinates](../../../../characteristic-coordinate.md)

$$
\xi=\sqrt x+\frac{y^{3/2}}3,\qquad \eta=\sqrt x-\frac{y^{3/2}}3.
$$

Their [Jacobian determinant](../../../../jacobian-determinant.md) is $-\sqrt y/(2\sqrt x)\ne0$, so they are valid independent coordinates. To see cancellation of the lower-order terms explicitly, first put $r=\sqrt x$, $s=y^{3/2}/3$ and $u(x,y)=U(r,s)$. The [chain rule](../../../../chain-rule.md) gives

$$
u_x=\frac{U_r}{2\sqrt x},\quad u_{xx}=\frac{U_{rr}}{4x}-\frac{U_r}{4x^{3/2}},\quad
u_y=\frac{\sqrt y}{2}U_s,\quad u_{yy}=\frac y4U_{ss}+\frac{U_s}{4\sqrt y}.
$$

Substitution cancels the first-derivative terms, leaving **$U_{ss}-U_{rr}=0$**. With $\xi=r+s$, $\eta=r-s$ and $U=V(\xi,\eta)$, the [characteristic normal form](../../../../characteristic-normal-form.md) is **$V_{\xi\eta}=0$**. Integrating once in each variable gives

$$
\boxed{u(x,y)=g\!\left(\sqrt x+\frac{y^{3/2}}3\right)+h\!\left(\sqrt x-\frac{y^{3/2}}3\right),}
$$

where $g,h$ are arbitrary twice continuously differentiable functions on the relevant coordinate intervals. This is a [curvilinear reduction to the one-dimensional wave equation](../../../../curvilinear-reduction-to-the-one-dimensional-wave-equation.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the differential equations 1 course of the University of Oxford](../../../split.md)
5. [Differential equations 1 course of the University of Oxford](../../../../differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
