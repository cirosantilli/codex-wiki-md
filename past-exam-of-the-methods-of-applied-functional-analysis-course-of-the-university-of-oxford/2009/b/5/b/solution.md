<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One form of [Schauder](../../../../../schauder-fixed-point-theorem.md)'s theorem says that if $M$ is a nonempty closed [bounded](../../../../../boundedness.md) convex [subset](../../../../../subset.md) of a [Banach space](../../../../../banach-space-split.md) and $T:M\to M$ is [continuous](../../../../../continuous-function.md) with relatively compact image, then $T$ has a [fixed point](../../../../../fixed-point.md).

For a [Schauder solution of a small Hammerstein integral equation](../../../../../schauder-solution-of-a-small-hammerstein-integral-equation.md), take $X=C([0,1])$ with the [supremum norm](../../../../../supremum-norm.md) and $M=\{u:\|u\|_\infty\le R\}$. This [set](../../../../../set-split.md) is nonempty, closed, [bounded](../../../../../boundedness.md) and convex. Put

$$
F_R=\max_{0\le y\le1,\ |z|\le R}|f(y,z)|,\qquad G_0=\max_{x,y\in[0,1]}|G(x,y)|,
\qquad\mu_0=\frac{R}{1+G_0F_R}>0.
$$

Both maxima are finite by [continuity](../../../../../continuous-function.md) on [compact sets](../../../../../compact-space.md). Define $(T_\mu u)(x)=\mu\int_0^1G(x,y)f(y,u(y))\,dy$. [Continuity](../../../../../continuous-function.md) and [uniform continuity](../../../../../uniform-continuity.md) of the [kernel](../../../../../kernel-of-a-linear-map-split.md) give $T_\mu u\in X$, and for $0<\mu\le\mu_0$,

$$
\|T_\mu u\|_\infty\le\mu G_0F_R\le R,
$$

so it is a self-map. This choice of $\mu_0$ also handles the case when either maximum is zero without division by zero.

If $u_n\to u$ uniformly in $M$, [uniform continuity](../../../../../uniform-continuity.md) of $f$ on $[0,1]\times[-R,R]$ makes $f(\cdot,u_n(\cdot))\to f(\cdot,u(\cdot))$ uniformly. The [integral](../../../../../integral-split.md) estimate then proves [continuity](../../../../../continuous-function.md) of $T_\mu$ in the [supremum norm](../../../../../supremum-norm.md). Moreover

$$
|(T_\mu u)(x)-(T_\mu u)(x')|\le\mu F_R\sup_y|G(x,y)-G(x',y)|,
$$

which tends to zero with $|x-x'|$ uniformly in $u\in M$. Thus the image is uniformly [bounded](../../../../../boundedness.md) and [equicontinuous](../../../../../equicontinuity.md). [Arzelà-Ascoli](../../../../../arzela-ascoli-theorem.md) states that such a family on a compact [interval](../../../../../interval-mathematics.md) has compact closure in the [supremum norm](../../../../../supremum-norm.md). Hence $T_\mu(M)$ is relatively compact, and [Schauder](../../../../../schauder-fixed-point-theorem.md) gives a [fixed point](../../../../../fixed-point.md) for each $\mu$ in the specified [interval](../../../../../interval-mathematics.md). Therefore **a [continuous](../../../../../continuous-function.md) solution with [supremum norm](../../../../../supremum-norm.md) at most $R$ exists**. The argument imposes no [Lipschitz](../../../../../lipschitz-continuity.md) hypothesis on $f$ and makes no uniqueness assertion.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
