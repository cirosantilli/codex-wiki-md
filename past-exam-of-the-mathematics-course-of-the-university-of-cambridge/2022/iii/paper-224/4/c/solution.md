<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A distribution on $\{1,2,\ldots\}$ must have $\mu\geq1$. For $\mu>1$, put $p=1/\mu$ and let

$$
G(k)=p(1-p)^{k-1}.
$$

For any mass function $P$ with mean $\mu$, [Gibbs inequality](../../../../../../gibbs-inequality.md) gives

$$
\begin{aligned}
D(P\Vert G)
&=-H(P)-\log_2p-(\mu-1)\log_2(1-p)\\
&=H(G)-H(P)\geq0.
\end{aligned}
$$

**Thus the [geometric distribution](../../../../../../geometric-distribution.md) uniquely maximizes entropy. For $\mu=1$, the only admissible law is the point mass at one, which is the limiting geometric case $p=1$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
