<h1 id="25k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Fatou's lemma](../../../../../../fatou-s-lemma.md) states that for nonnegative measurable $h_n$,

$$
\boxed{\int\liminf_n h_n\,d\mu\le\liminf_n\int h_n\,d\mu.}
$$

Indeed $g_n=\inf_{k\ge n}h_k$ is measurable, increases to $\liminf h_n$, and satisfies $g_n\le h_k$ for every $k\ge n$. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) gives $\int\liminf h_n=\lim_n\int g_n\le\lim_n\inf_{k\ge n}\int h_k$, proving the claim, including infinite values.

The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) states that if measurable $h_n\to h$ [almost everywhere](../../../../../../almost-everywhere.md) and $|h_n|\le g$ [almost everywhere](../../../../../../almost-everywhere.md) for one integrable nonnegative $g$, then $h$ is integrable and $\int h_n\to\int h$; in fact $\int|h_n-h|\to0$. Integrability follows from $|h|\le g$. For real functions, Fatou applied to $g+h_n$ gives $\int h\le\liminf\int h_n$, and applied to $g-h_n$ gives the reverse inequality against the upper limit. Thus the integrals converge. To obtain the stronger conclusion, Fatou applied to $2g-|h_n-h|\ge0$ gives $2\int g\le2\int g-\limsup\int|h_n-h|$, forcing the latter limit to be zero. Complex functions may be treated through their real and imaginary parts or the same absolute-difference argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [25K](../../25k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
