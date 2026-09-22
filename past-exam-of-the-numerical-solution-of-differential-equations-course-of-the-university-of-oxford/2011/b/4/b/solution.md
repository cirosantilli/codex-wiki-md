<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [four-point midpoint third derivative](../../../../../four-point-midpoint-third-derivative.md) uses the four values at $x_{j-1},x_j,x_{j+1},x_{j+2}$, centred at $x_{j+1/2}$. The [Taylor theorem](../../../../../taylor-s-theorem.md) about that midpoint gives

$$
\frac{u(x_{j+2})-3u(x_{j+1})+3u(x_j)-u(x_{j-1})}{h^3}
=u'''(x_{j+1/2})+\frac{h^2}{8}u^{(5)}(x_{j+1/2})+O(h^4).
$$

Thus, for $n\geq2$, take the $n-1$ interior equations

$$
\boxed{U_{j+2}-3U_{j+1}+3U_j-U_{j-1}=h^3f(x_{j+1/2}),\qquad j=1,\ldots,n-1.}
$$

Impose the two value conditions exactly, $U_0=\alpha$, $U_{n+1}=\beta$, and approximate the remaining condition with the second-order backward [finite difference](../../../../../finite-difference-split.md):

$$
\boxed{\frac{3U_{n+1}-4U_n+U_{n-1}}{2h}=\gamma.}
$$

This gives $n$ equations for $U_1,\ldots,U_n$. The endpoint [derivative](../../../../../derivative.md) formula equals $u'(b)-h^2u'''(b)/3+O(h^3)$, so its residual tends to zero along with those of the four-point equations. Every stencil lies within $[a,b]$; no unprescribed ghost value is introduced. The construction is therefore a consistent [finite difference method](../../../../../finite-difference-method.md) for all three boundary conditions.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
