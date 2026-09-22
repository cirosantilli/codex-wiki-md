<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [biregular graph](../../../../../../biregular-graph.md) assumption allows both [indicator functions](../../../../../../indicator-function.md) in the discrepancy to be balanced:

$$
\mathbb E_{x,y}G(x,y)1_A(x)1_B(y)-\alpha\beta\gamma
=\mathbb E_{x,y}H(x,y)(1_A(x)-\alpha)(1_B(y)-\beta).
$$

The [operator norm](../../../../../../operator-norm.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\left|\mathbb E H(1_A-\alpha)(1_B-\beta)\right|
\leq s\sqrt{\alpha(1-\alpha)\beta(1-\beta)}
\leq\frac{s}{4}.
$$

Consequently (iii)$\Rightarrow$(i) with $\boxed{c_1=c_3/4}$. Together with the previous sections, explicit constants for every direction are

$$
\begin{array}{c|cc}
\text{assumption}&\text{first consequence}&\text{second consequence}\\\hline
\text{(i), }c_1&c_3=(4c_1)^{1/3}&c_2=(4c_1)^{2/3}/4\\
\text{(ii), }c_2&c_3=c_2^{1/4}&c_1=c_2^{1/4}/4\\
\text{(iii), }c_3&c_1=c_3/4&c_2=c_3^2/4
\end{array}
$$

All these constants tend to zero with the initial constant and are independent of $|X|,|Y|$. This is the required equivalence for a [quasirandom bipartite graph](../../../../../../quasirandom-bipartite-graph.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
