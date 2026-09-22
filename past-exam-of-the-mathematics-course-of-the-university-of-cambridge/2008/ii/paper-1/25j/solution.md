<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) states that if measurable functions converge almost everywhere and their absolute values are bounded by a single [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md), their limit is integrable and their integrals converge to its integral.

Put $b_j=a_j/j$. The hypothesis makes $b_j$ summable. On the [positive integers](../../../../../positive-integer.md) with [counting measure](../../../../../counting-measure.md) define $f_n(j)=(j/n)b_j\mathbf1_{j\leq n}$. For each fixed $j$ it tends to zero and $0\leq f_n(j)\leq b_j$. Dominated convergence gives

$$
\boxed{\frac1n\sum_{j=1}^n a_j=\sum_jf_n(j)\longrightarrow0,}
$$

the stated [Kronecker lemma](../../../../../kronecker-lemma.md).

For a bounded interval union $B$, $S_j\sim N(0,j)$ has density bounded by $1/\sqrt{2\pi j}$. Hence $\mathbb P(S_j\in B)\leq |B|/\sqrt{2\pi j}$, and

$$
\mathbb E\sum_{j=1}^\infty\frac{\mathbf1_B(S_j)}j
\leq\frac{|B|}{\sqrt{2\pi}}\sum_{j=1}^\infty j^{-3/2}<\infty.
$$

By [Tonelli's theorem](../../../../../tonelli-theorem.md), the nonnegative series is finite [almost surely](../../../../../almost-sure-convergence.md). [Kronecker lemma](../../../../../kronecker-lemma.md) then makes the empirical occupation fraction of $B$ tend to zero. The family of finite rational-endpoint interval unions is countable, so intersecting their probability-one events proves simultaneous convergence for all of them. For the whole line, every indicator is one. Thus

$$
\boxed{m(B)=0\text{ for bounded }B\in F_0,\qquad m(\mathbb R)=1,\quad\text{almost surely}.}
$$

There is no countably additive [Borel measure](../../../../../borel-measure.md) extending these values: $\mathbb R=\bigcup_{n\geq1}(-n,n)$ would have measure zero by [continuity](../../../../../continuous-function.md) from below, contrary to its assigned measure one. The escaped empirical mass cannot be captured by a [probability](../../../../../probability.md) measure on the real line.

This is the [Gaussian random walk spends zero density of time in bounded sets](../../../../../gaussian-random-walk-spends-zero-density-of-time-in-bounded-sets.md) phenomenon.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
