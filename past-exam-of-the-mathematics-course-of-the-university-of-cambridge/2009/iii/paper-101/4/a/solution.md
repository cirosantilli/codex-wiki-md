<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau=T_{-a}\wedge T_b$ for the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md). From any interior point, $a+b$ successive $+1$ increments force exit through $b$. The conditional probability of this block is $2^{-(a+b)}$, so a blockwise [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) gives $\tau<\infty$ [almost surely](../../../../../../almost-sure-convergence.md).

Apply the bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $\tau\wedge n$. Since $S_n$ is a [martingale](../../../../../../martingale-split.md), $\mathbb E_0S_{\tau\wedge n}=0$. The stopped positions lie in $[-a,b]$, so the [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) gives $\mathbb E_0S_\tau=0$. If $h=\mathbb P_0(T_{-a}<T_b)$, nearest-neighbor jumps ensure $S_\tau=-a$ on that event and $S_\tau=b$ otherwise. Thus

$$
0=-ah+b(1-h),\qquad
\boxed{\mathbb P_0(T_{-a}<T_b)=\frac b{a+b}.}
$$

Next apply the bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the [square-minus-time martingale of a simple symmetric random walk](../../../../../../square-minus-time-martingale-of-a-simple-symmetric-random-walk.md):

$$
\mathbb E_0(\tau\wedge n)=\mathbb E_0S_{\tau\wedge n}^{,2}.
$$

Again the right side converges by the [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md), while the left side increases to $\mathbb E_0\tau$ by the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). Therefore

$$
\boxed{\mathbb E_0(T_{-a}\wedge T_b)
=a^2\frac b{a+b}+b^2\frac a{a+b}=ab.}
$$

This argument justifies passage to the unbounded [stopping time](../../../../../../stopping-time.md) rather than applying [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) without an integrability check.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
