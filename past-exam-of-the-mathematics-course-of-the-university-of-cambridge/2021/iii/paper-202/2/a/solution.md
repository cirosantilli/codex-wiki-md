<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The elementary discrete integration-by-parts identity is

$$
[X]^{(n)}_t=X_t^2-2M_t^{(n)}.
$$

By the supplied fact, $M^{(n)}\to M$ in $L^2$ of the uniform norm. Define

$$
[X]_t=X_t^2-2M_t.
$$

Then

$$
\mathbb E\sup_{t\geq0}|[X]^{(n)}_t-[X]_t|^2
=4\mathbb E\sup_{t\geq0}|M_t^{(n)}-M_t|^2\longrightarrow0,
$$

which proves i, while

$$
X^2-[X]=2M
$$

is an $L^2$-bounded martingale, proving ii.

Choose a subsequence converging uniformly almost surely. For $s<t$, all complete dyadic increments between $s$ and $t$ contribute nonnegative squares; only the two boundary increments can affect monotonicity, and they vanish uniformly by continuity of $X$. Passing to the limit gives $[X]_s\leq[X]_t$. Thus $[X]$ is nondecreasing and is the [quadratic variation](../../../../../../quadratic-variation.md) of $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
