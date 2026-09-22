<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [natural filtration](../../../../../../natural-filtration.md) $\mathcal F_n=\sigma(X_1,\ldots,X_n)$ of the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md). The event $\{T_1\leq n\}=\bigcup_{k=0}^n\{S_k=1\}$ belongs to $\mathcal F_n$, so $T_1$ is a [stopping time](../../../../../../stopping-time.md).

For a positive integer $m$, set $\tau_m=T_1\wedge T_{-m}$. This exit time from the finite interval is integrable: in each block of $m+1$ steps there is a [probability](../../../../../../probability.md) at least $2^{-(m+1)}$ of all steps being positive, which forces exit if it has not already occurred. Consequently the survival [probabilities](../../../../../../probability.md) have a geometric upper bound.

We use the bounded-time [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md): if $M$ is a [martingale](../../../../../../martingale-split.md) and $\sigma$ a bounded [stopping time](../../../../../../stopping-time.md), then $\mathbb E M_\sigma=\mathbb E M_0$. Apply it at $\tau_m\wedge n$ to $S_n$ and to the [square-minus-time martingale of a simple symmetric random walk](../../../../../../square-minus-time-martingale-of-a-simple-symmetric-random-walk.md) $S_n^2-n$. The stopped positions lie in $[-m,1]$, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) and [monotone convergence](../../../../../../monotone-convergence-theorem.md) give

$$
\mathbb E S_{\tau_m}=0,\qquad \mathbb E\tau_m=\mathbb E S_{\tau_m}^2.
$$

Writing $p_m=\mathbb P(T_1<T_{-m})$, the first equation becomes $p_m-m(1-p_m)=0$, hence $p_m=m/(m+1)$. The second gives $\mathbb E\tau_m=p_m+m^2(1-p_m)=m$. Since $\tau_m\leq T_1$, its [expectation](../../../../../../expected-value.md) satisfies $\mathbb E T_1\geq m$ for every $m$. Therefore

$$
\boxed{\mathbb E T_1=+\infty.}
$$

Nevertheless $\mathbb P(T_1<\infty)\geq p_m\to1$. Thus the [infinite mean first passage of a simple symmetric random walk](../../../../../../infinite-mean-first-passage-of-a-simple-symmetric-random-walk.md) occurs despite almost sure finiteness; using unrestricted optional stopping directly at $T_1$ would be unjustified.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
