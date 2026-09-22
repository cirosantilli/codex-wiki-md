<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a maximum of finitely many nonnegative quantities, its $p$th power is at most the sum of their $p$th powers. Hence the increment assumption gives

$$
\mathbb EA_n^p\leq\sum_{k=0}^{2^n-1}\mathbb E|X_{(k+1)2^{-n}}-X_{k2^{-n}}|^p
\leq C^p2^{n(1-p\beta)},\qquad
\|A_n\|_p\leq C2^{-n(\beta-1/p)}.
$$

By the [triangle inequality](../../../../../../../triangle-inequality.md) in the [Lp norm](../../../../../../../lp-norm.md), the partial sums defining $K_\alpha$ have norms bounded by a geometric series. [Monotone convergence](../../../../../../../monotone-convergence-theorem.md) of their $p$th powers gives

$$
\boxed{\|K_\alpha\|_p\leq\frac{2C}{1-2^{-(\beta-1/p-\alpha)}}<\infty.}
$$

In particular $K_\alpha$ is finite [almost surely](../../../../../../../almost-sure-convergence.md), so the preceding pathwise estimate has a common probability-one domain for all dyadic pairs.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 34](../../../../paper-34-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
