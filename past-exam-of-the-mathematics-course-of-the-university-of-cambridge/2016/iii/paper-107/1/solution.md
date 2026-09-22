<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Hopf boundary point lemma](../../../../../hopf-lemma.md) requires an [interior sphere condition](../../../../../interior-sphere-condition.md), strictness of the boundary maximum, and quantitative control of the [uniformly elliptic operator](../../../../../uniformly-elliptic-operator.md) near the contact point. Assume that $y\in\partial\Omega$, that $B_R(z)\subset\Omega$ and $\overline{B_R(z)}\setminus\{y\}\subset\Omega$, and that $|y-z|=R$. After shrinking the tangent [open ball](../../../../../open-ball.md), we may suppose that the coefficients are bounded there and that, for constants $0<\lambda\leq\Lambda$ and $B<\infty$,

$$
\lambda|\xi|^2\leq a^{ij}(x)\xi_i\xi_j\leq\Lambda|\xi|^2,
\qquad |b(x)|\leq B.
$$

The coefficient [matrix](../../../../../matrix.md) may be replaced by its [symmetric matrix](../../../../../symmetric-matrix.md) part because the [Hessian matrix](../../../../../hessian-matrix.md) is symmetric. Assume also that $u(x)<u(y)$ throughout the tangent [open ball](../../../../../open-ball.md). In the usual statement, one assumes $u(x)<u(y)$ throughout $\Omega$; when $\Omega$ is [connected](../../../../../connected-space.md), the [strong maximum principle for elliptic operators](../../../../../strong-maximum-principle-for-elliptic-operators.md) supplies this strictness from a nonconstant solution attaining its global maximum at $y$.

Put $\mathbf n=(y-z)/R$, the outward [unit normal](../../../../../unit-normal.md) of the tangent [open ball](../../../../../open-ball.md). With only the given [continuity](../../../../../continuous-function.md) at $y$, the precise conclusion is

$$
\boxed{\liminf_{t\downarrow0}\frac{u(y)-u(y-t\mathbf n)}{t}>0.}
$$

**If the outward normal derivative exists, it is strictly positive.** In particular, if $u$ is [continuously differentiable](../../../../../continuously-differentiable-function.md) up to $y$ and the domain has this outward [unit normal](../../../../../unit-normal.md), then $\partial_{\mathbf n}u(y)>0$. The stated $C^0$ boundary regularity alone does not assert existence of a [normal derivative](../../../../../normal-derivative.md).

For the proof, use the annulus $A=\{R/2<|x-z|<R\}$ and the [barrier for the Dirichlet problem](../../../../../barrier-for-the-dirichlet-problem.md)

$$
v(x)=e^{-k|x-z|^2}-e^{-kR^2}.
$$

Writing $q=x-z$, direct [differentiation](../../../../../differentiation.md) gives

$$
Lv=e^{-k|q|^2}\bigl(4k^2a^{ij}q_iq_j-2k\operatorname{tr}a-2kb\cdot q\bigr)
\geq e^{-k|q|^2}\bigl(k^2\lambda R^2-2k(n\Lambda+BR)\bigr).
$$

Choose $k>2(n\Lambda+BR)/(\lambda R^2)$, so that $Lv>0$ on $A$. On the inner sphere, [compactness](../../../../../compact-space.md) and the strict maximum give $m=\min_{|x-z|=R/2}(u(y)-u(x))>0$. Choose $\varepsilon>0$ with $\varepsilon\max_{|x-z|=R/2}v\leq m$. On the outer sphere $v=0$ and $u-u(y)\leq0$, including at $y$ by [continuity](../../../../../continuous-function.md). Consequently $w=u-u(y)+\varepsilon v$ has $Lw\geq0$ and nonpositive boundary values. The allowed comparison principle, or the [weak maximum principle for elliptic operators](../../../../../weak-maximum-principle-for-elliptic-operators.md), yields $w\leq0$ in $A$.

Along the inward radius this gives

$$
\frac{u(y)-u(y-t\mathbf n)}t\geq
\varepsilon\frac{e^{-k(R-t)^2}-e^{-kR^2}}t
\longrightarrow 2\varepsilon kR e^{-kR^2}>0.
$$

This proves the [Hopf boundary point lemma](../../../../../hopf-lemma.md). There is no sign restriction on $u(y)$ here, because the operator has no zeroth-order term.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 107](../../paper-107-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
