<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $a_n=n^{2(1-H)}$ and $b_n=n^{2(1-G)}$. Then $a_n/b_n=n^{2(G-H)}\to\infty$. The [large deviation principle](../../../../../../large-deviation-principle.md) on the whole space forces $\inf I=0$; compact [sublevel sets](../../../../../../sublevel-set.md) and [lower semicontinuity](../../../../../../lower-semicontinuity.md) make that [infimum](../../../../../../infimum.md) attained. The unique possible zero is therefore mu, and $I(\mu)=0$.

If a [closed set](../../../../../../closed-set.md) C contains mu, its new [infimum](../../../../../../infimum.md) rate is zero and the claimed upper bound follows from probabilities being at most one. If it excludes mu, then $\eta=\inf_CI>0$, possibly infinite: otherwise a sequence of rates tending to zero would have a [convergent subsequence](../../../../../../convergent-subsequence.md) in a compact [sublevel set](../../../../../../sublevel-set.md), with limit in C and zero rate, contradicting uniqueness. This is the fact that [a good rate function is separated from zero away from its minimizer](../../../../../../a-good-rate-function-is-separated-from-zero-away-from-its-minimizer.md).

Choose any $0<c<\eta$. The original upper bound gives $\log\mathbb P(X_n\in C)\leq-ca_n$ for all sufficiently large n. Thus

$$
\limsup_n b_n^{-1}\log\mathbb P(X_n\in C)\leq\lim_n-c\frac{a_n}{b_n}=-\infty=-\inf_CI'.
$$

Together these cases prove the **closed-set upper bound at the slower speed**, with rate zero only at mu. Its finite sublevels are the compact singleton $\{\mu\}$, so it is a [good rate function](../../../../../../good-rate-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
