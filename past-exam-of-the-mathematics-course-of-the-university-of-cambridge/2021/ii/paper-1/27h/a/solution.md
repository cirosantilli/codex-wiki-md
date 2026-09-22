<h1 id="27h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Fatou lemma](../../../../../../fatou-s-lemma.md) states that for any sequence $(f_n)$ of nonnegative measurable functions on a [measure space](../../../../../../measure-space.md),

$$
\boxed{\int\liminf_{n\to\infty}f_n\,d\mu
\leq
\liminf_{n\to\infty}\int f_n\,d\mu}.
$$

For the proof, define

$$
g_n=\inf_{k\geq n}f_k.
$$

Then $(g_n)$ is a nonnegative increasing sequence and

$$
g_n\uparrow\liminf_{k\to\infty}f_k.
$$

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) therefore gives

$$
\int\liminf_kf_k\,d\mu
=\lim_{n\to\infty}\int g_n\,d\mu.
$$

For each $k\geq n$, we have $g_n\leq f_k$, so [monotonicity of the Lebesgue integral](../../../../../../monotonicity-of-the-lebesgue-integral.md) yields

$$
\int g_n\,d\mu
\leq\inf_{k\geq n}\int f_k\,d\mu.
$$

Taking the limit in $n$ proves the asserted inequality and the [proof of Fatou lemma](../../../../../../proof-of-fatou-lemma.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27H](../../27h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
