<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the quoted event with, for example, $\alpha=1/4$, so at least $3k/4$ clean block means obey the uniform bound. Replacing at most $\epsilon n$ observations can corrupt at most $\epsilon n$ blocks. If $k\geq4\max\{n\epsilon,1\}$, at least $3k/4-\epsilon n\geq k/2$ block means remain both uncorrupted and good; adjusting constants handles equality and integer rounding. Their strict majority forces every projected median to obey the same uniform bound. Applying part b and absorbing fixed constants gives

$$
\|\widehat\mu(Z)-\mu_0\|_2
\leq c''\sqrt{
\frac{\max\{\operatorname{tr}(\Sigma),\|\Sigma\|_2k\}}n}
$$

with probability at least $1-e^{-c'k}$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
