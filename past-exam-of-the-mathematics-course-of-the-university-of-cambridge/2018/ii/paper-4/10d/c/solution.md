<h1 id="10d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

No classical one-query algorithm can determine $x_0$ with certainty. If it queries a string $x$ and receives $1$, then it knows $x_0=x$. But if it receives $0$, each of the other three strings remains compatible with the response. Randomization cannot remove this ambiguity when certainty is required. Thus

$$
\boxed{\text{one classical query is insufficient}.}
$$

Indeed, three adaptive classical queries are necessary and sufficient in the worst case: after three negative answers, the unqueried fourth string must be $x_0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
