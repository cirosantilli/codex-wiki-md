<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First let $1\leq p<\infty$, and take a [Cauchy sequence](../../../../../../cauchy-sequence.md) $f_j$ in the [Lp space](../../../../../../lp-space.md), with functions identified [almost everywhere](../../../../../../almost-everywhere.md). Choose a subsequence $f_{j_k}$ with $\|f_{j_{k+1}}-f_{j_k}\|_p\leq2^{-k}$ and put $a_k=f_{j_{k+1}}-f_{j_k}$. The [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\left\|\sum_{k=1}^N|a_k|\right\|_p\leq\sum_{k=1}^N2^{-k}\leq1.
$$

By the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), $A=\sum_{k\geq1}|a_k|$ belongs to $L^p$, and is finite almost everywhere. The series $f_{j_1}+\sum_{k\geq1}a_k$ therefore converges almost everywhere to an $L^p$ function $f$. Applying the same argument to each absolute tail yields

$$
\|f-f_{j_k}\|_p\leq\sum_{\ell\geq k}2^{-\ell}\longrightarrow0.
$$

The original sequence is Cauchy, so the triangle inequality extends convergence from this subsequence to the whole sequence.

For $p=\infty$, choose the same subsequence in [essential supremum](../../../../../../essential-supremum.md) norm. Outside one null set, all its difference bounds hold simultaneously:

$$
|a_k(x)|\leq2^{-k},\qquad |f_{j_1}(x)|\leq\|f_{j_1}\|_\infty.
$$

The series then converges uniformly on that full-measure set to a bounded measurable $f$, and $\|f-f_{j_k}\|_\infty\leq\sum_{\ell\geq k}2^{-\ell}$. Again the full sequence converges. Thus **every $L^p$, $1\leq p\leq\infty$, is a Banach space**, proving [completeness of Lp spaces](../../../../../../completeness-of-lp-spaces.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
