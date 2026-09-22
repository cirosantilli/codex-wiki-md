<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [travelling-wave reduction of a reaction-diffusion system](../../../../../travelling-wave-reduction-of-a-reaction-diffusion-system.md) of [Fisher's equation](../../../../../fisher-s-equation.md) is

$$
U''+cU'+U(1-U)=0,\qquad(U,U')(-\infty)=(1,0),\quad(U,U')(\infty)=(0,0).
$$

Multiplying by $U'$ and integrating gives $c\int_{\mathbb R}(U')^2dz=1/6$, so the decreasing invasion front has $c>0$. The [linearization](../../../../../linearization.md) at $U=0$ has spatial [eigenvalues](../../../../../eigenvalue.md)

$$
\lambda_\pm=\frac{-c\pm\sqrt{c^2-4}}2.
$$

For $0<c<2$ they are complex: approaching zero spirals in the $(U,U')$ plane and changes the sign of $U$, which is inadmissible for a density. Thus $c\geq2$ is necessary.

It is also sufficient. Write $V=U'$ and choose $\ell=(c-\sqrt{c^2-4})/2>0$. The triangle

$$
0\leq U\leq1,\qquad-\ell U\leq V\leq0
$$

is forward invariant for $U'=V$, $V'=-cV-U(1-U)$. On $V=0$, $V'\leq0$. On $V=-\ell U$,

$$
(V+\ell U)'=[c\ell-\ell^2-1]U+U^2=U^2\geq0.
$$

The boundary $U=1$ points left, and the boundary at $U=0$ consists only of the origin. The unstable branch from the saddle $(1,0)$ enters this triangle, where $U$ decreases and remains nonnegative. Its limiting state must have $V=0$ and $U(1-U)=0$; since it has left $U=1$, it tends to $(0,0)$. Therefore a monotone positive front exists for every $c\geq2$, including the double-root endpoint:

$$
\boxed{c_{\min}=2.}
$$

This is the [Fisher-KPP minimum wave speed](../../../../../fisher-kpp-minimum-wave-speed.md), obtained with an explicit invariant-region existence argument.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
