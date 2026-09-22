<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The variational terminology refers to the size of a neighborhood, rather than weak versus strong convergence in a [Banach space](../../../../banach-space-split.md). The definitions in the two numbered children give

$$
\boxed{\text{global minimizer}\Longrightarrow
\text{strong local minimizer}\Longrightarrow\text{weak local minimizer}.}
$$

The second implication holds because smallness in $W^{1,\infty}$ implies smallness in the [uniform norm](../../../../supremum-norm.md). Reverse implications need not hold.

For differentiable $f$ in its slope variable, define the [Weierstrass excess function](../../../../weierstrass-excess-function.md)

$$
E(x,y,p,q)=f(x,y,q)-f(x,y,p)-f_v(x,y,p)(q-p).
$$

The [strengthened Weierstrass condition](../../../../strengthened-weierstrass-condition.md) means that some $\delta>0$ gives

$$
\boxed{E(x,y,p,q)\geq0\quad\text{for all }x\in[a,b],\ q\in\mathbb R,
\quad |y-u(x)|<\delta,\quad|p-u'(x)|<\delta.}
$$

It requires support at nearby heights and nearby reference slopes, while the trial slope $q$ is arbitrary. Requiring this only exactly on the curve is the unstrengthened necessary condition.

A standard [Weierstrass sufficient condition](../../../../weierstrass-sufficient-condition.md) assumes the usual $C^2$ smoothness of $f$, $u\in\mathcal A\cap C^1$, the weak [Euler-Lagrange equation](../../../../euler-lagrange-equation.md), a coercively positive [second variation](../../../../second-variation.md), and the strengthened condition above. Explicitly, for some $c>0$,

$$
\delta^2I(u)[\eta,\eta]=\int_a^b
\bigl(f_{uu}\eta^2+2f_{uv}\eta\eta'+f_{vv}(\eta')^2\bigr)\,dx
\geq c\|\eta\|_{W^{1,2}}^2
$$

for zero-endpoint variations. Then **$u$ is a strong local minimizer**. If the excess is strictly positive for $q\ne p$ throughout the tube, the strong minimum is strict. The second-variation hypothesis supplies a neighboring field of extremals. Its slope $p(x,y)$ gives the comparison identity

$$
I(v)-I(u)=\int_a^b E(x,v(x),p(x,v(x)),v'(x))\,dx\geq0
$$

for uniformly close admissible $v$. This explains how the condition controls competitors with large derivatives.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the calculus of variations course of the University of Oxford](../../../split.md)
5. [Calculus of variations course of the University of Oxford](../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
