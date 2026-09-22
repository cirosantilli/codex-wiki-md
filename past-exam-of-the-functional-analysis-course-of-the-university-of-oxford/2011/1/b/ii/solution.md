<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $1<p<\infty$ and $q=p/(p-1)$. The dual of $\ell^p$ is $\ell^q$. For every $a\in\ell^q$, $\langle a,e_n\rangle=a_n\to0$, so $e_n\rightharpoonup0$ weakly. A [compact operator](../../../../../compact-operator-split.md) sends a weakly convergent [sequence](../../../../../sequence.md) to a norm-convergent [sequence](../../../../../sequence.md) with the corresponding limit. Indeed, any failure of $\|Te_n\|\to0$ would give a [subsequence](../../../../../subsequence.md) bounded away from zero, with a further norm-convergent [subsequence](../../../../../subsequence.md) by [compactness](../../../../../compact-space.md); weak [continuity](../../../../../continuous-function.md) of $T$ forces that [norm](../../../../../norm.md) limit to be zero, a contradiction. The condition is therefore **necessary**.

For failure of sufficiency, partition the positive integers into consecutive blocks

$$
B_k=\{k(k-1)/2+1,\ldots,k(k+1)/2\},\qquad |B_k|=k,
$$

and define the [block averaging compactness counterexample](../../../../../block-averaging-compactness-counterexample.md)

$$
\boxed{(Tx)_k=k^{-1/q}\sum_{j\in B_k}x_j.}
$$

By [Hölder's inequality](../../../../../holder-s-inequality.md), $|(Tx)_k|^p\leq\sum_{j\in B_k}|x_j|^p$. Summing over disjoint blocks shows $\|Tx\|_p\leq\|x\|_p$, so $T$ is bounded. If $j\in B_k$, then $Te_j=k^{-1/q}e_k$; as $j\to\infty$, also $k\to\infty$, so $\|Te_j\|_p\to0$.

However, the [vectors](../../../../../vector.md) $x^{(k)}=k^{-1/p}\mathbf1_{B_k}$ have [norm](../../../../../norm.md) one and satisfy $Tx^{(k)}=e_k$. Distinct output [vectors](../../../../../vector.md) have distance $2^{1/p}$, so this bounded [sequence](../../../../../sequence.md) of inputs has no norm-convergent image [subsequence](../../../../../subsequence.md). Thus **$T$ is not [compact](../../../../../compact-space.md)**.

To connect with the hint, define $(Uy)_j=k^{-1/q}y_k$ for $j\in B_k$. Then $U:\ell^q\to\ell^q$ is an isometry, and the dual pairing calculation gives $T=U^*$. The [vectors](../../../../../vector.md) $Ue_k$ have disjoint supports and [norm](../../../../../norm.md) one. The direct estimates above establish the counterexample without relying only on the hint.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the functional analysis course of the University of Oxford](../../../../split.md)
6. [Functional analysis course of the University of Oxford](../../../../../functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
