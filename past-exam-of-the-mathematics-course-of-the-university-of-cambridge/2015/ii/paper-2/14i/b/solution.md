<h1 id="14i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Induction with Pascal's identity gives the [binomial upper bound for a Ramsey number](../../../../../../binomial-upper-bound-for-a-ramsey-number.md) $R(s,t)\leq\binom{s+t-2}{s-1}$. Thus $R(s)\leq\binom{2s-2}{s-1}\leq4^{s-1}$, proving **$R(s)=O(4^s)$**.

For the lower bound, take a [binomial random graph](../../../../../../binomial-random-graph.md) $G(n,1/2)$. The expected total number of $s$-cliques and independent $s$-sets is

$$
2\binom ns2^{-\binom s2}\leq2\frac{n^s}{s!}2^{-s(s-1)/2}.
$$

For $n=\lfloor2^{s/2}/2\rfloor$, this is at most $2^{1-s/2}/s!<1$ for all sufficiently large $s$. Some [graph](../../../../../../graph-split.md) therefore has neither forbidden set, so $R(s)>n$. This proves **$R(s)=\Omega(2^{s/2})$** by the [probabilistic method](../../../../../../probabilistic-method.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14I](../../14i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
