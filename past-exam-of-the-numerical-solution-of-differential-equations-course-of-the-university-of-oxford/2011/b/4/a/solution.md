<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the second-order [boundary value problem](../../../../../boundary-value-problem-split.md), introduce an unknown initial slope $s$ and solve the [initial value problem](../../../../../initial-value-problem.md) $u'=v$, $v'=g(x,u,v)$ with $u(a)=\alpha$, $v(a)=s$. Its endpoint mismatch is $F(s)=u(b;s)-\beta$. The [shooting method](../../../../../shooting-method.md) seeks a root $F(s)=0$; in general the dependence of the flow on $s$ is nonlinear. A sign-changing bracket for a continuous $F$ allows the [bisection method](../../../../../bisection-method.md), provided the intervening initial value solutions exist up to $b$.

For [Newton's method](../../../../../newton-s-method-in-optimization.md), solve the [parameter sensitivity equation](../../../../../parameter-sensitivity-equation.md) alongside the trajectory. With $z=\partial_su$ and $w=\partial_sv$,

$$
z'=w,\qquad w'=g_u z+g_{u'}w,\qquad z(a)=0,\quad w(a)=1.
$$

Then $F'(s)=z(b)$ and the update is $\boxed{s_{\mathrm{new}}=s-F(s)/z(b)}$ whenever $z(b)\ne0$.

For the third-order problem, shooting from $a$ leaves both $u'(a)$ and $u''(a)$ unknown, requiring two shooting parameters to satisfy two right-endpoint conditions. Shooting backwards from $b$ already knows $u(b)=\beta$ and $u'(b)=\gamma$; only $u''(b)$ is unknown, with the single residual $u(a)-\alpha$. **Backward shooting reduces the nonlinear solve from two scalar unknowns to one.** This parameter-count advantage does not by itself guarantee numerical stability of backward integration.

## ↑ Ancestors (13)

1. [A](../a.md)
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
