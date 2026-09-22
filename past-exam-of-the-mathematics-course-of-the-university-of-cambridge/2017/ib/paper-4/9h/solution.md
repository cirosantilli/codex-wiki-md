<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Let $S_0=0$ and let each increment of the [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md) be uniformly chosen from $\{\pm e_1,\pm e_2,\pm e_3\}$. A return requires an even number of steps. In $2n$ steps returning to zero, let $a,b,c$ be the respective numbers of positive steps in the three directions; there must also be $a,b,c$ negative steps, so $a+b+c=n$. Counting step sequences gives

$$
u_{2n}:=\mathbb P_0(S_{2n}=0)=\frac{(2n)!}{6^{2n}}\sum_{a+b+c=n}\frac1{a!^2b!^2c!^2}
=\frac{\binom{2n}{n}}{4^n}\sum_{a+b+c=n}\left(\frac{n!}{3^na!b!c!}\right)^2.
$$

The terms $p_{abc}=n!/(3^na!b!c!)$ form a [multinomial distribution](../../../../../multinomial-distribution.md), so $\sum p_{abc}^2\leq(\max p_{abc})\sum p_{abc}=\max p_{abc}$. The permitted combinatorial inequalities give $\binom{2n}{n}/4^n\leq C_1n^{-1/2}$ and $\max_{a+b+c=n}p_{abc}\leq C_2/n$ for $n\geq1$. The second bound also follows by noting that the largest [multinomial coefficient](../../../../../multinomial-coefficient.md) occurs when $a,b,c$ differ by at most one and then applying [Stirling formula](../../../../../stirling-formula.md). Thus

$$
\boxed{u_{2n}\leq Cn^{-3/2},\qquad u_{2n+1}=0,\qquad \sum_{j\geq0}\mathbb P_0(S_j=0)<\infty}.
$$

To prove the origin is a [transient state](../../../../../transient-state.md), let $q$ be the [probability](../../../../../probability.md) of at least one return after time zero. The [Strong Markov property](../../../../../strong-markov-property.md) at successive returns gives $\mathbb P(N\geq k)=q^k$ for the number $N$ of later returns. Therefore $\mathbb E(N+1)=\sum_j u_j$ would be infinite if $q=1$. The bound forces $q<1$, proving that the origin is a [transient state](../../../../../transient-state.md). Translation invariance gives the same conclusion at every lattice point. The coordinate walks need not be treated as independent; the counting via [multinomial coefficients](../../../../../multinomial-coefficient.md) already incorporates their dependence.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
