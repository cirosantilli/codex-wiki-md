<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [bounded-variation space](../../../../../../function-of-bounded-variation-on-a-domain.md) carries the [norm](../../../../../../norm.md) $\|u\|_{BV}=\|u\|_{L^1(\Omega)}+|Du|(\Omega)$. Its [weak-star convergence in BV](../../../../../../weak-star-convergence-in-bv.md) is characterized by

$$
\boxed{u_k\to u\text{ in }L^1(\Omega),\qquad Du_k\overset{*}{\rightharpoonup}Du\text{ in }\mathcal M(\Omega;\mathbb R^n).}
$$

The second condition means convergence of the [vector measure](../../../../../../vector-measure.md) pairings against every $\varphi\in C_0(\Omega;\mathbb R^n)$. Equivalently, [strong convergence](../../../../../../norm-convergence.md) in $L^1$ together with $\sup_k|Du_k|(\Omega)<\infty$ suffices: [integration by parts](../../../../../../integration-by-parts.md) identifies the limit on smooth compactly supported tests, and [uniform approximation](../../../../../../uniform-approximation-split.md) extends this to $C_0$ tests.

The [bounded-variation compactness](../../../../../../bounded-variation-compactness.md) theorem says that

$$
\boxed{\sup_k\bigl(\|u_k\|_{L^1(\Omega)}+|Du_k|(\Omega)\bigr)<\infty}
$$

guarantees a [subsequence](../../../../../../subsequence.md) convergent in [weak-star convergence in BV](../../../../../../weak-star-convergence-in-bv.md) on a bounded [Lipschitz domain](../../../../../../lipschitz-domain.md). This is the uniform criterion for relative sequential compactness. If asking only for the existence of one convergent [subsequence](../../../../../../subsequence.md), the exact condition is the existence of a BV-bounded [subsequence](../../../../../../subsequence.md), equivalently $\liminf_k\|u_k\|_{BV}<\infty$. The entire sequence need not be bounded: alternating zero functions and constants tending to infinity gives a simple example. Conversely, a convergent [subsequence](../../../../../../subsequence.md) has bounded $L^1$ [norm](../../../../../../norm.md) and bounded [total variation seminorm](../../../../../../total-variation-seminorm-on-a-domain.md) by the [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) for its derivative-measure pairings.

## ↑ Ancestors (11)

1. [I](../i.md)
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
