<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a [bounded BV extension operator](../../../../../../bounded-bv-extension-operator.md) for the bounded [Lipschitz domain](../../../../../../lipschitz-domain.md). Extend $u_k$ to $w_k\in BV(\mathbb R^n)$, supported in one fixed [compact set](../../../../../../compact-space.md), with $\|w_k\|_{BV(\mathbb R^n)}\le C_\Omega\|u_k\|_{BV(\Omega)}$. Such an extension is obtained by reflection in Lipschitz boundary charts, a [partition of unity](../../../../../../partition-of-unity.md) and a fixed [cutoff function](../../../../../../cutoff-function.md). A naive zero extension must also charge its boundary-trace jump; it cannot discard that contribution.

Let $M$ bound these [norms](../../../../../../norm.md) and let $w_{k,\epsilon}=w_k*\rho_\epsilon$ be their [mollifications](../../../../../../mollification.md). The [BV mollification error estimate](../../../../../../bv-mollification-error-estimate.md) gives

$$
\|w_{k,\epsilon}-w_k\|_1\le\epsilon|Dw_k|(\mathbb R^n)\le\epsilon M.
$$

The [variation measure](../../../../../../variation-measure.md) here is on $\mathbb R^n$. The printed lemma's $|Dw|(\Omega)$ needs this correction unless it also assumes all the [derivative](../../../../../../derivative.md) mass lies in $\Omega$: a nonconstant bump supported outside $\overline\Omega$ disproves its literal wording. The correct estimate follows by averaging the [BV translation estimate](../../../../../../bv-translation-estimate.md) $\|w(\cdot-h)-w\|_1\le|h||Dw|(\mathbb R^n)$ over a mollifier supported in $|h|\le\epsilon$.

For each fixed $\epsilon>0$, [convolution](../../../../../../convolution.md) gives uniform bounds

$$
\|w_{k,\epsilon}\|_\infty\le M\|\rho_\epsilon\|_\infty,\qquad \|\nabla w_{k,\epsilon}\|_\infty\le M\|\nabla\rho_\epsilon\|_\infty.
$$

The [mollifications](../../../../../../mollification.md) have common [compact support](../../../../../../compact-support.md) and are uniformly [equicontinuous](../../../../../../equicontinuity.md). The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) supplies a uniformly convergent [subsequence](../../../../../../subsequence.md) at each scale $\epsilon=1/m$. A diagonal [subsequence](../../../../../../subsequence.md) converges at every one of those scales. For two late members of that [subsequence](../../../../../../subsequence.md),

$$
\|w_k-w_\ell\|_1\le2M/m+\|w_{k,1/m}-w_{\ell,1/m}\|_1.
$$

First choose large $m$, then late $k,\ell$; the sequence is a [Cauchy sequence](../../../../../../cauchy-sequence.md) in $L^1$. Its limit $w$ belongs to the [BV space](../../../../../../function-of-bounded-variation-on-a-domain.md) because the [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md) is [sequentially lower semicontinuous](../../../../../../sequential-lower-semicontinuity.md). Uniform [derivative](../../../../../../derivative.md) bounds and [integration by parts](../../../../../../integration-by-parts.md) give $Dw_k\overset{*}{\rightharpoonup}Dw$. Restriction to $\Omega$ proves the required [weak-star convergence in BV](../../../../../../weak-star-convergence-in-bv.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
