<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Proceed by [mathematical induction](../../../../../../mathematical-induction.md) on $n$. The cases $n=0,1$ are immediate. Given a [symmetric chain decomposition of a Boolean lattice](../../../../../../symmetric-chain-decomposition-of-a-boolean-lattice.md) $\mathcal P([n-1])$, consider one of its chains

$$
A_r\subset A_{r+1}\subset\cdots\subset A_{n-1-r},
\qquad |A_j|=j.
$$

It produces the two chains

$$
A_r\subset\cdots\subset A_{n-1-r}
\subset A_{n-1-r}\cup\{n\}
$$

and, when nonempty,

$$
A_r\cup\{n\}\subset A_{r+1}\cup\{n\}
\subset\cdots\subset A_{n-2-r}\cup\{n\}.
$$

The first runs from rank $r$ to rank $n-r$, and the second from rank $r+1$ to rank $n-1-r$; both endpoint ranks sum to $n$. They are disjoint and together contain the old chain both without and with $n$. Doing this for every old chain partitions $\mathcal P([n])$ into symmetric chains.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
