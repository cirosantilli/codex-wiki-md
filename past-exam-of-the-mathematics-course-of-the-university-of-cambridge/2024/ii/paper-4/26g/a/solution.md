<h1 id="26g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Uniform integrability means

$$
\lim_{K\to\infty}\sup_n
\mathbb E\bigl[|X_n|\mathbf1_{\{|X_n|>K\}}\bigr]=0.
$$

If $\sup_n\mathbb E|X_n|^p=C<\infty$ for $p>1$, then

$$
\mathbb E[|X_n|\mathbf1_{|X_n|>K}]
\leq K^{1-p}\mathbb E|X_n|^p\leq CK^{1-p},
$$

proving uniform integrability. For a counterexample, let $X_n=n$ with probability $1/n$ and zero otherwise. Then $\mathbb E|X_n|=1$, but for every $K$ and $n>K$ the tail expectation is one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26G](../../26g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
