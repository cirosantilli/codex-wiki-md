<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\delta=C-\mu>0$, and first suppose $\sigma>0$. For the infinite-horizon contraction, use the usual [sublinear path space for fluid queues](../../../../../../sublinear-path-space-for-fluid-queues.md),

$$
\mathcal C_0=\{f\in C([0,\infty)):f(0)=0,\ f(t)/(1+t)\to0\},
\qquad \|f\|_{\rm sl}=\sup_{t\geq0}\frac{|f(t)|}{1+t}.
$$

We interpret the supplied path-space [large deviation principle](../../../../../../large-deviation-principle.md) in this norm, or in a topology with the same workload-continuity property. The paper does not specify its norm explicitly; mere convergence on compact time intervals would not justify an infinite-horizon contraction.

Define the [queue workload](../../../../../../workload-of-a-queue.md) functional

$$
R(f)=\sup_{t\geq0}\{\sigma f(t)-\delta t\}.
$$

It is finite and nonnegative on the [sublinear path space for fluid queues](../../../../../../sublinear-path-space-for-fluid-queues.md). Here is the required continuity argument. Fix $f$ and choose $T\geq1$ so that $|\sigma f(t)|\leq\delta t/4$ for $t\geq T$. If $\|g-f\|_{\rm sl}<\delta/(4\sigma)$, then for $t\geq T$,

$$
\sigma g(t)-\delta t
\leq\frac{\delta t}{4}+\frac{\delta(1+t)}4-\delta t
=\frac{\delta}{4}-\frac{\delta t}{2}<0.
$$

The corresponding expression for $f$ is also negative there, whereas at zero both are zero. Each [supremum](../../../../../../supremum.md) can therefore be restricted to $[0,T]$, giving

$$
|R(g)-R(f)|\leq\sigma(1+T)\|g-f\|_{\rm sl}.
$$

Thus $R$ is a [continuous map](../../../../../../continuous-map.md); this proof also shows why the negative drift is essential.

Substituting $t=Ns$ into the [queue workload](../../../../../../workload-of-a-queue.md) gives

$$
\frac{r(X)}N=\sup_{s\geq0}\left\{\sigma\frac{Z(Ns)}N-\delta s\right\}
=R\!\left(\frac{Z(N\,\cdot)}N\right).
$$

The [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) says that a continuous image of a family with [good rate function](../../../../../../good-rate-function.md) $I$ has the same [large-deviation speed](../../../../../../large-deviation-speed.md) and [good rate function](../../../../../../good-rate-function.md) obtained by minimizing $I$ over each fibre. Consequently

$$
\boxed{\text{speed }N^{2(1-H)},\qquad
J(q)=\inf_{\{f:R(f)=q\}}I(f)\quad(q\geq0),\qquad J(q)=+\infty\quad(q<0).}
$$

In particular $J(0)=0$: $Z/\sqrt L\to0$ in the path norm almost surely, so the given [large deviation principle](../../../../../../large-deviation-principle.md) and [lower semicontinuity](../../../../../../lower-semicontinuity.md) give $I(0)=0$, and $R(0)=0$. If $\sigma=0$, the [queue workload](../../../../../../workload-of-a-queue.md) is identically zero and the [rate function](../../../../../../rate-function.md) is zero at zero and infinite elsewhere. No unspecified [variance](../../../../../../variance-split.md) normalization of the [fractional Brownian motion](../../../../../../fractional-brownian-motion.md) is needed for this variational answer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
