<h1 id="3/1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The small-parameter limit depends on [data compatibility with the regularizer domain](../../../../../../../data-compatibility-with-the-regularizer-domain.md). Set

$$
m=\inf_{v\in\operatorname{dom}J}D(v),\qquad 0\leq m\leq D(0).
$$

For every such $v$, optimality gives

$$
m\leq D(u_\alpha)\leq\Phi_{\alpha,f}(u_\alpha)
\leq D(v)+\alpha J(v).
$$

Taking the upper limit as $\alpha\downarrow0$ and then the [infimum](../../../../../../../infimum.md) over $v$ proves $\Phi_{\alpha,f}(u_\alpha)\to m$. Its two nonnegative contributions above $m$ must vanish, yielding the general result

$$
\boxed{D(u_\alpha)\longrightarrow m,\qquad
\alpha J(u_\alpha)\longrightarrow0.}
$$

In particular, the requested zero-misfit limit holds when $f\in\overline{K(\operatorname{dom}J)}$. A sufficient condition is an exact solution $v$ with $Kv=f$ and $J(v)<\infty$; then

$$
0\leq D(u_\alpha)\leq\alpha J(v),\qquad
0\leq\alpha J(u_\alpha)\leq\alpha J(v)\longrightarrow0.
$$

**Membership of $f$ in $\mathcal R(K)$ alone is insufficient.** Take $\mathcal U=\mathcal V=\mathbb R$, $K=I$, $f=1$, and $J$ the [indicator functional of a constraint set](../../../../../../../indicator-functional-of-a-constraint-set.md) $\{0\}$. All positive-parameter objectives are [proper extended-real functions](../../../../../../../proper-extended-real-function.md) with [coercivity](../../../../../../../coercive-function.md) and [sequential lower semicontinuity](../../../../../../../sequential-lower-semicontinuity.md), with the unique minimizer $u_\alpha=0$, yet $D(u_\alpha)=1/2$ for every $\alpha$. Thus the first printed limit needs compatibility with the regulariser's [effective domain](../../../../../../../effective-domain.md); the second limit remains true under the given assumptions.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
