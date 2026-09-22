<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The [Liouville approximation theorem](../../../../../liouville-approximation-theorem.md) says that if $\alpha$ is an irrational [algebraic number](../../../../../algebraic-number.md) of degree $d$, there is $c_\alpha>0$ such that $|\alpha-p/q|\ge c_\alpha q^{-d}$ for all integers $p$ and $q\ge1$. To see the source of the bound, a degree-$d$ integer [minimal polynomial](../../../../../minimal-polynomial.md) $P$ gives $q^dP(p/q)$ a nonzero integer. On a fixed neighbourhood of $\alpha$, the [mean value theorem](../../../../../mean-value-theorem.md) bounds $|P(p/q)|$ by a constant times $|p/q-\alpha|$; outside that neighbourhood a smaller uniform constant suffices.

Let $\alpha$ denote the factorial-denominator sum and let $p_N/q_N$ be its partial sum through $N$, with $q_N=10^{N!}$ for $N\ge2$. This is an integer numerator even though $0!=1!=1$ makes the first two terms equal. Positivity and the rapid increase of factorial exponents imply

$$
0<\alpha-\frac{p_N}{q_N}<2\,10^{-(N+1)!}=2q_N^{-(N+1)}.
$$

For example the first omitted term is $10^{-(N+1)!}$ and every succeeding factorial exponent increases by at least one, giving a geometric tail bound less than $10/9$ times that first term.

First $\alpha$ is irrational: if $\alpha=a/b$, the positive difference from a partial sum is at least $1/(bq_N)$, contradicting this bound for sufficiently large $N$. If it were algebraic of any fixed degree $d$, [Liouville approximation theorem](../../../../../liouville-approximation-theorem.md) would require $c_\alpha q_N^{-d}<2q_N^{-(N+1)}$, again impossible for large $N$. Hence $\boxed{\alpha\text{ is transcendental}.}$

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
