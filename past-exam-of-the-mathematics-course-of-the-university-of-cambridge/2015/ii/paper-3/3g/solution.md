<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Order the prescribed lengths as $l_1\leq\cdots\leq l_N$. Construct a [prefix code](../../../../../prefix-code.md) on the binary tree. At depth $l_i$, previously assigned codewords exclude $\sum_{j<i}2^{l_i-l_j}$ of the $2^{l_i}$ vertices. The [Kraft inequality](../../../../../kraft-mcmillan-inequality.md) implies

$$
\sum_{j<i}2^{l_i-l_j}+1\leq2^{l_i},
$$

so an available vertex can be assigned to the next symbol. None of the assigned words is a prefix of another. Reading each word up to the next assigned vertex gives unique decoding, so this constructs the required [uniquely decodable code](../../../../../decipherable-code.md).

For completeness the same length inequality is necessary even for a [uniquely decodable code](../../../../../decipherable-code.md) which is not a [prefix code](../../../../../prefix-code.md). Write $K=\sum_a2^{-l(a)}$ and $L=\max_a l(a)$. For $r$ successive symbols, distinct symbol strings have distinct concatenated codewords. At total length $j$ there are at most $2^j$ such strings. Therefore

$$
K^r=\sum_{j=r}^{rL}N_j2^{-j}\leq rL.
$$

Taking $r$th roots and letting $r\to\infty$ gives $K\leq1$. This is the [McMillan inequality](../../../../../mcmillan-inequality.md).

Set $q(a)=2^{-l(a)}/K$. The [relative entropy](../../../../../kullback-leibler-divergence.md) inequality gives

$$
\mathbb E l(A)-H(A)=\sum_a p(a)\log_2\frac{p(a)}{q(a)}-\log_2K\geq0.
$$

Here [Shannon entropy](../../../../../information-entropy.md) uses base $2$, with $0\log0=0$. The [relative entropy](../../../../../kullback-leibler-divergence.md) is nonnegative, with equality precisely when the two [probability distributions](../../../../../probability-distribution.md) coincide; this follows from $\log t\leq t-1$. Consequently **equality holds exactly when**

$$
\boxed{K=1\quad\hbox{and}\quad p(a)=2^{-l(a)}\ \hbox{for every }a.}
$$

In particular all alphabet symbols must have positive probability for equality with finite prescribed lengths.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
