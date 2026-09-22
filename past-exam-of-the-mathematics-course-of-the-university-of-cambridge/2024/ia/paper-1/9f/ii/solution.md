<h1 id="9f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First suppose $L>0$. Taking logarithms,

$$
\log a_n
=\log a_1+\sum_{k=1}^{n-1}
\log\left(\frac{a_{k+1}}{a_k}\right).
$$

Divide by $n$. Since the summands tend to $\log L$, their Cesàro means also tend to $\log L$. Hence

$$
\frac1n\log a_n\to\log L,
$$

and exponentiation gives $a_n^{1/n}\to L$.

If $L=0$, then for every $\varepsilon>0$ the ratios are eventually at most $\varepsilon$, so $a_n\leq C\varepsilon^n$ for a suitable constant $C$. Thus

$$
\limsup a_n^{1/n}\leq\varepsilon.
$$

Letting $\varepsilon\downarrow0$ proves the [ratio limit implies root limit](../../../../../../ratio-limit-implies-root-limit.md) in all cases.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
