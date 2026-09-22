<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Write the principal part as $e^{2y}u_{xx}-u_{yy}$. The [characteristic curves](../../../characteristic-curve.md) satisfy

$$
e^{2y}(dy)^2-(dx)^2=0,
$$

or $dx/dy=\pm e^y$. Integration gives $x+e^y=\text{constant}$ and $x-e^y=\text{constant}$. Thus take $\xi=x+e^y$, $\eta=x-e^y$. Their [Jacobian determinant](../../../jacobian-determinant.md) is $-2e^y\ne0$, and their image is $\xi>\eta$.

For $u(x,y)=U(\xi,\eta)$, the [chain rule](../../../chain-rule.md) gives

$$
u_{xx}=U_{\xi\xi}+2U_{\xi\eta}+U_{\eta\eta},\qquad
u_y=e^y(U_\xi-U_\eta),
$$



$$
u_{yy}=e^{2y}(U_{\xi\xi}-2U_{\xi\eta}+U_{\eta\eta})
+e^y(U_\xi-U_\eta).
$$

The first-derivative terms cancel exactly. The [canonical form of a second-order partial differential equation](../../../canonical-form-of-a-second-order-partial-differential-equation.md) is

$$
4e^{2y}U_{\xi\eta}=0,\qquad U=F(\xi)+G(\eta).
$$

On $y=0$, $F(x+1)+G(x-1)=x$. Differentiating this condition in $x$ and using $u_y=1$ gives

$$
F'(x+1)+G'(x-1)=1,\qquad F'(x+1)-G'(x-1)=1.
$$

Hence $F'=1$ and $G'=0$. Substitution into the value condition fixes their combined constant and yields

$$
\boxed{u(x,y)=x+e^y-1.}
$$

Direct substitution verifies the PDE and both initial data. The cancellation illustrates a [hyperbolic equation reduced by an exponential characteristic coordinate](../../../hyperbolic-equation-reduced-by-an-exponential-characteristic-coordinate.md).

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2008](../../2008-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
