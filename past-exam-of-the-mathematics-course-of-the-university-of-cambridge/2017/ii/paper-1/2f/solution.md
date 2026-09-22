<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The [Liouville approximation theorem](../../../../../liouville-approximation-theorem.md) states that an irrational [algebraic number](../../../../../algebraic-number.md) $\alpha$ of degree $d\ge2$ satisfies $|\alpha-a/b|\ge C_\alpha b^{-d}$ for all integers $a$ and $b\ge1$, for some $C_\alpha>0$. The constant is independent of the rational approximation.

The required condition is **infinitely many of the coefficients equal one**. If only finitely many do, the [series](../../../../../series-mathematics.md) is a finite sum of [rational numbers](../../../../../rational-number.md). Conversely let $\alpha$ be the sum with infinitely many nonzero terms. Its truncation $s_N$ has denominator dividing $q_N=10^{N!}$. For $N\ge2$, its strictly positive tail satisfies

$$
0<\alpha-s_N\le\sum_{j=N+1}^\infty10^{-j!}
<2\,10^{-(N+1)!}=2q_N^{-(N+1)}.
$$

If $\alpha=a/b$ were rational, the distinct fractions $\alpha,s_N$ would have distance at least $1/(bq_N)$, contradicting the tail bound for large $N$. Thus $\alpha$ is irrational. If it were algebraic of fixed degree $d$, apply the [Liouville approximation theorem](../../../../../liouville-approximation-theorem.md) to $s_N$. Even if its reduced denominator is smaller than $q_N$, the lower bound is at least $C_\alpha q_N^{-d}$. The displayed upper bound contradicts this as $N\to\infty$. Hence

$$
\boxed{\alpha\text{ is transcendental}\iff\#\{n:\zeta_n=1\}=\infty}.
$$

The coincidence $0!=1!$ changes only the first rational contribution and has no effect on this criterion.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
