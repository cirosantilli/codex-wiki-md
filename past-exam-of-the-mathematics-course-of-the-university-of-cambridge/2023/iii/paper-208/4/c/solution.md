<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Z_i$ be the longest increasing subsequence length after deleting coordinate $i$. Then $0\leq Z-Z_i\leq1$. Choose one longest increasing subsequence $I$ of length $Z$. If deleting $i$ reduces the optimum, then $i$ must belong to $I$; consequently at most $Z$ coordinates can satisfy $Z-Z_i=1$. Hence

$$
\sum_{i=1}^n(Z-Z_i)^2\leq Z,
$$

so $Z$ is a [weakly self-bounding function](../../../../../../weakly-self-bounding-function.md). The [variance bound for a weakly self-bounding function](../../../../../../variance-bound-for-a-weakly-self-bounding-function.md) gives

$$
\boxed{\operatorname{Var}(Z)leq\mathbb EZ.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
