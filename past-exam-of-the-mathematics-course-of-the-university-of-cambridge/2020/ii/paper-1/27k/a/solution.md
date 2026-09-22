<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The space $L^2(X,\mathcal F,\nu)$ consists of equivalence classes, modulo equality almost everywhere, of measurable real functions satisfying

$$
\int_X|f|^2\,d\nu<\infty.
$$

It has inner product and induced norm

$$
\langle f,g\rangle=\int_Xfg\,d\nu,
\qquad
\|f\|_2=\left(\int_X|f|^2\,d\nu\right)^{1/2}.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) makes the inner product finite and verifies the norm axioms.

To prove completeness, let $(f_n)$ be Cauchy and choose a subsequence such that

$$
\|f_{n_{k+1}}-f_{n_k}\|_2\le2^{-k}.
$$

By the triangle inequality, the partial sums

$$
g_N=\sum_{k=1}^N|f_{n_{k+1}}-f_{n_k}|
$$

have uniformly bounded $L^2$ norm. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) shows that their pointwise limit $g$ belongs to $L^2$ and is finite almost everywhere. The telescoping series therefore converges almost everywhere to a measurable function $f$, and

$$
\|f-f_{n_m}\|_2
\le\sum_{k=m}^{\infty}2^{-k}\longrightarrow0.
$$

The original Cauchy sequence then converges to $f$ in $L^2$. Thus the result that an [L2 space is a Hilbert space](../../../../../../l2-space-is-a-hilbert-space.md) gives

$$
\boxed{L^2(X,\mathcal F,\nu)\text{ is a Hilbert space}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
