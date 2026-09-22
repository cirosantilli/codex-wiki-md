<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a nonzero [Laurent series](../../../../../../laurent-series.md) let $\operatorname{ord}_t$ be its least exponent. Choose $|x|=p^{-\operatorname{ord}_t(x)}$ and $|0|=0$. This is a multiplicative [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md), and its [valuation ring](../../../../../../valuation-ring.md) is $\mathbb F_p[[t]]$.

Take

$$
\boxed{L=\mathbb F_{p^f}((u)),\qquad t\longmapsto u^e.}
$$

If $\gamma_1,\ldots,\gamma_f$ is an $\mathbb F_p$-basis of $\mathbb F_{p^f}$, the elements $\gamma_i u^j$, $1\le i\le f$, $0\le j<e$, form a $K$-basis of $L$. To see this, group the exponents of each Laurent series modulo $e$ and then expand its coefficients in the constant-field basis. Uniqueness of those two expansions proves linear independence. Thus $[L:K]=ef$.

Its [valuation ring](../../../../../../valuation-ring.md) is $\mathbb F_{p^f}[[u]]$, with maximal ideal $(u)$ and residue field $\mathbb F_{p^f}$. Moreover $\operatorname{ord}_u(t)=e$, so the [ramification index](../../../../../../ramification-index.md) is $e$ and the [residue degree](../../../../../../residue-degree.md) is $f$. The unique extending absolute value is explicitly

$$
\boxed{\left|\sum_{n\ge n_0}a_nu^n\right|_L=p^{-\min\{n:a_n\ne0\}/e},\qquad |0|_L=0.}
$$

This restricts to the chosen absolute value because $\operatorname{ord}_u(x)=e\operatorname{ord}_t(x)$ on $K$. The [prescribed ramification and residue degree for a Laurent series field](../../../../../../prescribed-ramification-and-residue-degree-for-a-laurent-series-field.md) construction works even when $p\mid e$; separability is not required in the question.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
