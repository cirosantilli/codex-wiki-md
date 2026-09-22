<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In position-velocity variables $(u,v)$, the scalar right-hand side is

$$
F(x,u,v)=\frac{v^2}{u}+2xv.
$$

Its only relevant singularity is $u=0$. The initial state $(x,u,v)=(0,1,1)$ is separated from it. For an explicit application of part (a), take $h=1$ and $k=1/2$ in the [L1 norm](../../../../l1-norm.md). On the resulting [closed ball](../../../../closed-ball.md), $1/2\leq u,v\leq3/2$, and $|x|\leq1$.

The [partial derivatives](../../../../partial-derivative.md) obey

$$
|F_u|=\frac{v^2}{u^2}\leq9,\qquad
|F_v|=\left|\frac{2v}{u}+2x\right|\leq8.
$$

The ball is [convex](../../../../convex-function.md), so integrating these [partial derivatives](../../../../partial-derivative.md) along a segment between two states gives the uniform [Lipschitz condition](../../../../lipschitz-continuity.md)

$$
|F(x,u,v)-F(x,\widetilde u,\widetilde v)|
\leq9\bigl(|u-\widetilde u|+|v-\widetilde v|\bigr).
$$

Continuity holds on the whole slab, and

$$
|F|\leq\frac{(3/2)^2}{1/2}+2\cdot1\cdot\frac32=\frac{15}2,
\qquad\|(v,F)\|_1\leq9.
$$

Thus $L=9$, $M\leq9$, and the choice $\boxed{\eta=1/20}$ satisfies the self-map and contraction bounds in part (a). This proves **a unique solution on $[-1/20,1/20]$**, with $y$ bounded away from zero there.

There is also a useful exact representation. Where $y>0$, set $q=y'/y$, the [logarithmic derivative](../../../../logarithmic-derivative.md). Differentiation cancels the quadratic term:

$$
q'=\frac{y''}{y}-\frac{(y')^2}{y^2}=2xq,\qquad q(0)=1.
$$

Solving this [first-order linear differential equation](../../../../first-order-linear-differential-equation.md) gives $q=e^{x^2}$, and a second integration yields

$$
\boxed{y(x)=\exp\left(\int_0^x e^{t^2}\,dt\right).}
$$

This [function](../../../../function-split.md) is positive and smooth for every real $x$, satisfies both initial data, and verifies the original [ordinary differential equation](../../../../ordinary-differential-equation.md) by direct differentiation. It therefore extends the unique local solution to the entire real line. The [logarithmic-derivative reduction of a second-order equation](../../../../logarithmic-derivative-reduction-of-a-second-order-equation.md) explains why this apparently nonlinear example is explicitly integrable by [integration](../../../../integral-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
