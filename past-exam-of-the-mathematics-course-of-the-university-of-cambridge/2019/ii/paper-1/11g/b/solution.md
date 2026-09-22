<h1 id="11g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S$ be the support of the weight-$d$ codeword $x$, and let $\pi_S$ delete all coordinates in $S$. Its kernel consists of codewords supported in $S$. If $0\ne y\in\ker\pi_S$, then $\operatorname{wt}(y)\geq d$ but $|S|=d$, so $y$ is nonzero in every coordinate of $S$. Over $\mathbb F_2$ this forces $y=x$. Hence

$$
\ker\pi_S=\langle x\rangle
$$

has dimension one, and the [punctured code](../../../../../../punctured-code.md) $C'=\pi_S(C)$ has length $n-d$ and rank $k-1$ by the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md).

To bound its minimum distance, take $y\in C$ whose puncture $y'$ is nonzero. If $y$ has $r$ nonzero coordinates in $S$, then $y+x$ has $d-r$ there, while both words have the same $\operatorname{wt}(y')$ nonzero coordinates outside $S$. Both $y$ and $y+x$ are nonzero codewords, so

$$
\operatorname{wt}(y')+r\geq d,
\qquad
\operatorname{wt}(y')+d-r\geq d.
$$

Adding gives $2\operatorname{wt}(y')\geq d$, and therefore

$$
\boxed{d'\geq\left\lceil\frac d2\right\rceil}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11G](../../11g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
