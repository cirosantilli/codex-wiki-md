<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $X=\mu+\sigma Z$, where $Z$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md). Apply [Gaussian integration by parts](../../../../../../stein-s-lemma-probability.md) to $g(z)=U'(\mu+\sigma z)$:

$$
\mathbb E[ZU'(X)]=\mathbb E[g'(Z)]=\sigma\mathbb E[U''(X)].
$$

Since $X-\mu=\sigma Z$,

$$
\boxed{\mathbb E[U'(X)(X-\mu)]=\sigma^2\mathbb E[U''(X)]}.
$$

The polynomial growth assumption and decay of the [normal distribution](../../../../../../normal-distribution.md) density justify the integration by parts.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
