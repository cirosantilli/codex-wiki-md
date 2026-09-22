<h1 id="12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $X_1$ and $X_2$ denote the first and second labels. [Sampling with replacement](../../../../../sampling-with-replacement.md) restores the bag before the second draw, so conditioning on $X_1=x$ only specifies the threshold. For $1\leq x\leq g$, there are $x$ qualifying green balls and $x$ qualifying red balls. For $g<x\leq r$, every green ball and the first $x$ red balls qualify. Hence the requested [conditional probability](../../../../../conditional-probability.md) is

$$
\boxed{\mathbb P(X_2\leq x\mid X_1=x)=
\begin{cases}
\dfrac{2x}{g+r},&1\leq x\leq g,\\[4pt]
\dfrac{g+x}{g+r},&g<x\leq r.
\end{cases}}
$$

The formulas agree at $x=g$ and give one at $x=r$. Labels outside the possible first-draw range do not define a conditioning event of positive [probability](../../../../../probability.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
