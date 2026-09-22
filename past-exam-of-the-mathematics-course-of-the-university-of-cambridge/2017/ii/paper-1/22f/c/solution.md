<h1 id="22f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $1<p<\infty$, apply [Fatou lemma](../../../../../../fatou-s-lemma.md) to the nonnegative [sequence](../../../../../../sequence.md) $|f_n|^p$, which converges pointwise to $|f|^p$:

$$
\int_{\mathbb R}|f|^p\,d\lambda
\le\liminf_n\int_{\mathbb R}|f_n|^p\,d\lambda\le M^p.
$$

For $p=\infty$, each inequality $\|f_n\|_\infty\le M$ fails pointwise only on a null [set](../../../../../../set-split.md). Outside the union of these countably many null [sets](../../../../../../set-split.md), $|f_n(x)|\le M$ for every $n$, so the pointwise limit also satisfies $|f(x)|\le M$. Therefore in both cases

$$
\boxed{f\in L^p(\mathbb R),\qquad\|f\|_p\le M}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
