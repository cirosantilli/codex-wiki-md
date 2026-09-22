<h1 id="2h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The sum is nonempty because $A$ and $B$ are nonempty. It is a [bounded set](../../../../../../bounded-set.md): if $|a|\leq M_A$ and $|b|\leq M_B$, then $|a+b|\leq M_A+M_B$.

To prove that it is a [closed set](../../../../../../closed-set.md), let $x_j=a_j+b_j\in A+B$ be a [convergent sequence](../../../../../../convergent-sequence.md) with $x_j\to x$. By the [Heine-Borel theorem](../../../../../../heine-borel-theorem.md), $A$ is a [compact set](../../../../../../compact-space.md), so $(a_j)$ has a [convergent subsequence](../../../../../../convergent-subsequence.md) $a_{j_r}\to a\in A$. Then

$$
b_{j_r}=x_{j_r}-a_{j_r}\longrightarrow x-a.
$$

Since $B$ is closed, $x-a\in B$, and hence $x=a+(x-a)\in A+B$. Therefore $A+B$ is nonempty, closed and bounded, so $A+B\in\mathcal K$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2H](../../2h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
