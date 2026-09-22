<h1 id="25j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Fatou's lemma](../../../../../../fatou-s-lemma.md) states that nonnegative [measurable functions](../../../../../../measurable-function.md) satisfy

$$
\boxed{\int\liminf_nf_n\,d\mu\le\liminf_n\int f_n\,d\mu}.
$$

To prove it, put $h_n=\inf_{k\ge n}f_k$. These measurable nonnegative functions increase to $\liminf f_n$. By the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), $\int\liminf f_n=\lim_n\int h_n$. Since $h_n\le f_k$ for every $k\ge n$, one has $\int h_n\le\inf_{k\ge n}\int f_k$. Taking the limit proves the inequality, including extended infinite integrals.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [25J](../../25j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
