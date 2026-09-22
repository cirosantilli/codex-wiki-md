<h1 id="25k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $A_n=\int f_n^+$, $B_n=\int f_n^-$, $A=\int f^+$ and $B=\int f^-$. Almost-everywhere convergence gives $f_n^\pm\to f^\pm$, so [Fatou's lemma](../../../../../../fatou-s-lemma.md) gives $A\le\liminf A_n$ and $B\le\liminf B_n$. The given norm condition is $A_n+B_n\to A+B$. Consequently

$$
\limsup A_n\le A+B-\liminf B_n\le A,
$$

and the symmetric argument bounds $\limsup B_n\le B$. Combining upper and lower limits proves

$$
\boxed{\int f_n^+\,d\mu\to\int f^+\,d\mu,\qquad\int f_n^-\,d\mu\to\int f^-\,d\mu.}
$$

No common integrable dominating function for $f_n$ has been assumed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
