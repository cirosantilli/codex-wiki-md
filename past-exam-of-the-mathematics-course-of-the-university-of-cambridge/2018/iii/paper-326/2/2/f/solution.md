<h1 id="2/2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Iterated Tikhonov regularization](../../../../../../../iterated-tikhonov-regularization.md) update is the [proximal operator](../../../../../../../proximal-operator.md) step

$$
\boxed{u_\delta^{(k+1)}=\underset{u\in\mathcal U}{\operatorname{argmin}}
\left\{\frac12\|Ku-f^\delta\|^2
+\frac1{2\tau}\|u-u_\delta^{(k)}\|^2\right\}.}
$$

The objective has [coercivity](../../../../../../../coercive-function.md) and is weakly [sequentially lower semicontinuous](../../../../../../../sequential-lower-semicontinuity.md) and [strongly convex](../../../../../../../strongly-convex-function.md), so the [direct method in the calculus of variations](../../../../../../../direct-method-in-the-calculus-of-variations.md) and [uniqueness of a minimizer of a strictly convex function](../../../../../../../uniqueness-of-a-minimizer-of-a-strictly-convex-function.md) give existence and uniqueness. Its [gradient](../../../../../../../gradient.md) equation is

$$
K^*(Ku-f^\delta)+\tau^{-1}(u-u_\delta^{(k)})=0,
$$

which is exactly $(I+\tau K^*K)u=u_\delta^{(k)}+\tau K^*f^\delta$. The second term penalizes the change from the previous iterate, rather than the [norm](../../../../../../../norm.md) of $u$ relative to zero.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
