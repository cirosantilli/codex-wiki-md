<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the $r$ distinct [codewords](../../../../../../codeword.md) be $x^{(1)},\ldots,x^{(r)}\in\mathbb F_2^N$. No [linearity](../../../../../../linearity.md) assumption is needed. Sum their [Hamming distances](../../../../../../hamming-distance.md) over unordered distinct pairs:

$$
S=\sum_{1\leq i<j\leq r}d(x^{(i)},x^{(j)}).
$$

Each summand is at least the [minimum Hamming distance](../../../../../../minimum-distance-of-a-code.md) $\delta$, so $S\geq\delta r(r-1)/2$.

For coordinate $a$, let $m_a$ be the number of [codewords](../../../../../../codeword.md) whose $a$th bit is $1$. Exactly $m_a(r-m_a)$ unordered pairs differ at that coordinate. Summing coordinate contributions gives

$$
S=\sum_{a=1}^Nm_a(r-m_a)
\leq\sum_{a=1}^N\frac{r^2}{4}
=\frac{Nr^2}{4},
$$

since $m_a(r-m_a)=r^2/4-(m_a-r/2)^2$. Combining the two bounds and dividing by $r>0$ gives $2\delta(r-1)\leq Nr$, hence $r(2\delta-N)\leq2\delta$. Under $2\delta>N$, division is legitimate, proving the [Plotkin bound](../../../../../../plotkin-bound.md)

$$
\boxed{r\leq\frac{2\delta}{2\delta-N}}.
$$

Because $r$ is an integer, it also satisfies the floor of the right-hand side. The binary alphabet is essential to the coordinate count; this proof applies to arbitrary [binary block codes](../../../../../../binary-block-code.md), not just linear ones.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
