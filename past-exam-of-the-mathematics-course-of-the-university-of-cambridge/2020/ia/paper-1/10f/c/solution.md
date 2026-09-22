<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Construct the nested index sequences inductively. Start with $N^{(0)}=(1,2,\ldots)$. Having chosen $N^{(i-1)}$, apply the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) to the bounded sequence of $i$th coordinates along those indices, and let $N^{(i)}$ be an increasing subsequence along which that coordinate converges. Because each new sequence is nested inside all earlier ones, coordinates $1,\ldots,i$ all converge along $N^{(i)}$.

Now take the [diagonal subsequence argument](../../../../../../diagonal-subsequence-argument.md)

$$
m_j=n_j^{(j)}.
$$

Nestedness implies

$$
m_{j+1}=n_{j+1}^{(j+1)}\geq n_{j+1}^{(j)}>n_j^{(j)}=m_j,
$$

so $(m_j)$ is strictly increasing. For every fixed $i$, the tail $(m_j)_{j\geq i}$ is a subsequence of $N^{(i)}$; hence $(x_{m_j}^{(i)})$ converges. This single diagonal subsequence works for every coordinate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
