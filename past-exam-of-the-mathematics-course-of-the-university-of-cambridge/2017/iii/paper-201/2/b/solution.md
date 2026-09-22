<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $m\geq1$, the increments have exponential moment

$$
\mathbb E2^{X_1}=\frac67\,2^{-1}+\frac17\,2^2=1.
$$

Thus $Z_n=2^{S_n}$ is an [exponential martingale of a random walk](../../../../../../exponential-martingale-of-a-random-walk.md) relative to the natural [filtration](../../../../../../filtration-probability-theory.md). We justify its stopping limit. From any surviving state in $(-m,m)$, a block of $2m$ successive increments all equal to $-1$ forces an exit. The block has probability $q=(6/7)^{2m}>0$, independently of the preceding increments. The [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) gives

$$
\mathbb P(T>2m\ell)\leq(1-q)^\ell,
$$

so $T$ is finite [almost surely](../../../../../../almost-sure-convergence.md) and has finite [expectation](../../../../../../expected-value.md).

At the lower exit $S_T=-m$ exactly; at the upper exit $S_T$ is either $m$ or $m+1$. Before exit the same overall bound $-m\leq S_{n\wedge T}\leq m+1$ holds. Hence $Z_{n\wedge T}$ is bounded by $2^{m+1}$, uniformly in $n$. The bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $\mathbb E Z_{n\wedge T}=Z_0=1$, and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) now yields

$$
\boxed{\mathbb E2^{S_T}=1.}
$$

Allowing the upper overshoot by one is essential; the terminal state need not equal $m$ on upper exit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
