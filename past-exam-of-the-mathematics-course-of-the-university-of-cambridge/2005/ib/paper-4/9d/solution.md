<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

Let $S_m$ be the [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md) started at the origin. Odd-time returns are impossible by parity. A return in $2n$ steps requires equal numbers of positive and negative steps along each axis. If these paired counts are $i,j,k$ with $i+j+k=n$, counting the possible step arrangements gives

$$
p_{2n}:=P(S_{2n}=0)=\frac{(2n)!}{6^{2n}}\sum_{i+j+k=n}\frac1{i!^2j!^2k!^2}.
$$

Define $q_{ijk}=n!/(3^ni!j!k!)$. These are [multinomial distribution](../../../../../multinomial-distribution.md) probabilities and sum to one. Rearranging the return formula gives

$$
p_{2n}=\frac{\binom{2n}{n}}{4^n}\sum_{i+j+k=n}q_{ijk}^2
\leq\frac{\binom{2n}{n}}{4^n}\max_{i+j+k=n}q_{ijk}.
$$

The maximum occurs when the three counts differ by at most one: if $i\geq j+2$, replacing $(i,j)$ by $(i-1,j+1)$ multiplies $q$ by $i/(j+1)>1$. At balanced counts, [Stirling's formula](../../../../../stirling-formula.md) gives $\max q=O(n^{-1})$; the exponential factors cancel because each count is $n/3+O(1)$, and the square-root factorial factors leave one inverse power of $n$. The same formula gives $\binom{2n}{n}/4^n\sim(\pi n)^{-1/2}$. Hence

$$
\boxed{p_{2n}=O(n^{-3/2}),\qquad \sum_{m\geq0}P(S_m=0)<\infty.}
$$

This is the [multinomial collision proof of three-dimensional walk transience](../../../../../multinomial-collision-proof-of-three-dimensional-walk-transience.md). The sum is the expected total number of visits to the origin. If the probability of returning after departure were one, the [Strong Markov property](../../../../../strong-markov-property.md) at successive returns would make every successive return finite almost surely, giving infinitely many visits and contradicting that finite expectation. Thus the origin is a [transient state](../../../../../transient-state.md). Translation invariance gives the same conclusion at every lattice point: **the three-dimensional walk is transient**.

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
