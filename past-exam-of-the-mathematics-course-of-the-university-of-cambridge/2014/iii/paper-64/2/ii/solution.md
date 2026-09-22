<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $t\in\mathbb R$, define the set functional

$$
F_t(E)=\alpha\operatorname{Per}(E;\Omega)+\int_E(t-f)\,dx.
$$

The [ROF level-set formulation](../../../../../../rof-level-set-formulation.md) states that the unique [minimizer](../../../../../../global-minimizer.md) of $J(u)=\|u-f\|_2^2/2+\alpha\operatorname{TV}(u)$ has [superlevel sets](../../../../../../superlevel-set.md) minimizing $F_t$ for almost every $t$. Conversely, an admissible $u$ with minimizing [superlevel sets](../../../../../../superlevel-set.md) is the ROF [minimizer](../../../../../../global-minimizer.md). Thus the concise characterization is

$$
\boxed{\hat u\text{ minimizes ROF}\iff\{\hat u>t\}\in\arg\min_E F_t(E)\text{ for a.e. }t.}
$$

The [signed layer-cake identity for quadratic fidelity](../../../../../../signed-layer-cake-identity-for-quadratic-fidelity.md) and the [coarea formula for BV functions](../../../../../../coarea-formula-for-bv-functions.md) give

$$
J(u)-\frac12\|f\|_2^2=\int_{\mathbb R}\bigl[F_t(\{u>t\})-F_t(E_t^0)\bigr]dt,\qquad E_t^0=\begin{cases}\Omega,&t<0,\\\varnothing,&t\ge0.\end{cases}
$$

Indeed $u^2/2-fu=\int_{\mathbb R}(t-f)(\chi_{\{u>t\}}-\chi_{\{0>t\}})dt$ pointwise. Its absolute integral is bounded by $u^2/2+|fu|$, so [Fubini's theorem](../../../../../../fubini-s-theorem.md) applies for $u,f\in L^2$. The negative-level baseline is essential; integrating the unadjusted $F_t$ would generally diverge.

Each $F_t$ attains its minimum. A [minimizing sequence](../../../../../../minimizing-sequence.md) of [indicator functions](../../../../../../indicator-function.md) has bounded $L^1$ [norm](../../../../../../norm.md), and comparison with the empty set bounds its perimeter by an $L^1$ forcing bound. [Bounded-variation compactness](../../../../../../bounded-variation-compactness.md) supplies a limiting [indicator function](../../../../../../indicator-function.md). The forcing integral converges by [dominated convergence](../../../../../../dominated-convergence-theorem.md), while [relative perimeter](../../../../../../relative-perimeter.md) is [sequentially lower semicontinuous](../../../../../../sequential-lower-semicontinuity.md).

For $s<t$, the supplied comparison lemma applied to $(f-t)/\alpha<(f-s)/\alpha$ makes every selected [minimizer](../../../../../../global-minimizer.md) $A_t$ contained in $A_s$ up to a [null set](../../../../../../null-set.md). The [comparison of perimeter minimizers with ordered forcing](../../../../../../comparison-of-perimeter-minimizers-with-ordered-forcing.md) also follows directly: compare $A_t$ with $A_t\cap A_s$, compare $A_s$ with $A_t\cup A_s$, add and use [submodularity of relative perimeter](../../../../../../submodularity-of-relative-perimeter.md) to obtain $(t-s)|A_t\setminus A_s|\le0$.

Select [minimizers](../../../../../../global-minimizer.md) at rational levels, remove their countably many exceptional [null sets](../../../../../../null-set.md), and reconstruct $v(x)=\sup\{q\in\mathbb Q:x\in A_q\}$. The strict [superlevel set](../../../../../../superlevel-set.md) is $\{v>t\}=\bigcup_{q>t}A_q$. This union also minimizes $F_t$: take $q\downarrow t$, use monotone $L^1$ convergence of its [indicator functions](../../../../../../indicator-function.md) and [sequential lower semicontinuity](../../../../../../sequential-lower-semicontinuity.md), and note that $m(t)=\min_EF_t(E)$ satisfies $|m(t)-m(s)|\le|\Omega||t-s|$.

To justify finite energy before assuming it, clip this reconstruction to $v_M\in[-M,M]$. Comparison with the empty set gives $\alpha\operatorname{Per}(E_t;\Omega)\le\int_\Omega|t-f|$ uniformly on a bounded interval of levels. Since $v_M=-M+\int_{-M}^M\chi_{E_t}\,dt$, pairing with compactly supported test-field divergences bounds its [total variation seminorm](../../../../../../total-variation-seminorm-on-a-domain.md) by $\int_{-M}^M\operatorname{Per}(E_t;\Omega)dt<\infty$. Thus $v_M$ belongs to the [BV space](../../../../../../function-of-bounded-variation-on-a-domain.md) before applying the [coarea formula for BV functions](../../../../../../coarea-formula-for-bv-functions.md). The layer-cake argument on the finite interval $[-M,M]$ shows $J(v_M)\le J(T_Mw)$ for every finite-energy competitor $w$, where $T_M$ is clipping. In particular $w=0$ bounds the $L^2$ [norms](../../../../../../norm.md) and variations uniformly. [Fatou's lemma](../../../../../../fatou-s-lemma.md) excludes infinite values of $v$ on a positive-measure set. [Bounded-variation compactness](../../../../../../bounded-variation-compactness.md) and [weak convergence](../../../../../../weak-convergence.md) in $L^2$ identify an admissible limit $v$. For any fixed competitor, $T_Mw\to w$ in $L^2$ and its variation tends to that of $w$, by [bounded-variation contraction under clipping](../../../../../../bounded-variation-contraction-under-clipping.md) and [sequential lower semicontinuity](../../../../../../sequential-lower-semicontinuity.md). Thus $J(v)\le J(w)$.

The [quadratic fidelity](../../../../../../quadratic-fidelity.md) is [strictly convex](../../../../../../strictly-convex-function.md), so every ROF [minimizer](../../../../../../global-minimizer.md) equals $v$ [almost everywhere](../../../../../../almost-everywhere.md) and has the selected minimizing [superlevel sets](../../../../../../superlevel-set.md). Conversely, for any $u$ whose levels minimize $F_t$, integrate the levelwise inequality against any competitor's levels in the displayed identity to obtain $J(u)\le J(w)$. This proves both directions for signed as well as nonnegative data.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
