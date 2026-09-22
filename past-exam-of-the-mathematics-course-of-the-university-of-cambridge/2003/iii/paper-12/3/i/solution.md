<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $M=2m$ and $a_i=\binom{d_i}{2}$. Use the [configuration model](../../../../../../configuration-model.md): give vertex $i$ exactly $d_i$ labelled [half-edges](../../../../../../half-edge-of-a-graph.md) and choose a uniform [perfect matching](../../../../../../perfect-matching.md) of all $M$ half-edges. There are

$$
\frac{M!}{2^m m!}=\frac{(2m)_m}{2^m}
$$

pairings, with $(2m)_m$ denoting a [falling factorial](../../../../../../falling-factorial.md). Each allowed [simple graph](../../../../../../simple-graph.md) has exactly $\prod_i d_i!$ representations: at every vertex, assign its incident graph edges bijectively to its labelled half-edges. Therefore its enumeration reduces to the probability that a pairing is simple and avoids $G_0$.

Count three kinds of prescribed bad patterns. A loop pattern consists of a pair of half-edges at one vertex. A double-edge pattern consists of two half-edges at each of two distinct vertices and one of their two cross-pairings. A forbidden-edge pattern consists of one half-edge at each endpoint of an edge of $G_0$. Let their respective counts in the random pairing be $Z_L,Z_D,Z_F$. Simplicity and avoidance are equivalent to $Z=Z_L+Z_D+Z_F=0$, including exclusion of triple edges because those contain double-edge patterns.

A prescribed collection of $t$ disjoint half-edge pairs occurs with [probability](../../../../../../probability.md)

$$
\frac1{(M-1)(M-3)\cdots(M-2t+1)}.
$$

Consequently the bad-pattern [expected values](../../../../../../expected-value.md) are

$$
\begin{aligned}
\mathbb EZ_L&=\frac{\sum_i a_i}{M-1}=\frac\lambda2+o(1),\\
\mathbb EZ_D&=\frac{2\sum_{i<j}a_i a_j}{(M-1)(M-3)}=\frac{\lambda^2}4+o(1),\\
\mathbb EZ_F&=\frac{\sum_{ij\in E(G_0)}d_id_j}{M-1}=\mu+o(1).
\end{aligned}
$$

Here $\lambda=(\sum_i a_i)/m$ and $\mu=M^{-1}\sum_{ij\in E(G_0)}d_id_j$, as in the PDF. Since $1\leq d_i\leq\Delta$ and $G_0$ has bounded [maximum degree](../../../../../../maximum-degree.md), $M=\Theta(n)$ and all three means are uniformly bounded. For the double-edge estimate, $\sum_i a_i^2=O(n)$, so its contribution after division by $M^2$ is $o(1)$.

We now give the moment-counting step rather than assume independence. For each fixed $h$, expand the [factorial moment](../../../../../../factorial-moment.md) $\mathbb E(Z)_h$ as the sum over ordered distinct bad patterns. Collections on disjoint vertex sets have, by the displayed pairing probability, joint probabilities equal to the product probabilities times $1+O(1/n)$. Their total contribution is

$$
\left(\frac\lambda2+\frac{\lambda^2}4+\mu\right)^h+o(1).
$$

Deleting collections with a shared vertex changes the independent-product sum by $O(1/n)$, since all ordinary and forbidden vertex degrees are bounded.

For actual joint probabilities of overlapping patterns, incompatible uses of a half-edge give zero. Compatible collections with no shared paired edge lose at least one free vertex choice, without reducing the number of required pairs, so contribute $O(1/n)$. A shared paired edge can occur only between two double-edge patterns or between a double-edge pattern and a forbidden-edge pattern. In the first case their union requires at least three parallel paired edges: there are $O(n^2)$ endpoint choices and probability $O(n^{-3})$. In the second case the endpoint pair must be an edge of $G_0$: there are only $O(n)$ choices and at least two required pairs, giving $O(n^{-1})$. Adding further patterns in a fixed collection does not remove this deficit: a disjoint addition contributes bounded order, while an addition to an existing cluster has only bounded half-edge choices unless it supplies new free vertices, compensated by its new required pairs. Summing the finitely many overlap types for fixed $h$ therefore gives $o(1)$. Thus, with $\Lambda=\lambda/2+\lambda^2/4+\mu$,

$$
\mathbb E(Z)_h=\Lambda^h+o(1)\quad\text{for every fixed }h.
$$

The [Bonferroni inequalities](../../../../../../bonferroni-inequalities.md) bracket $\Pr(Z=0)$ by the odd and even partial sums of $\sum_h(-1)^h\mathbb E(Z)_h/h!$. The means $\Lambda$ are bounded, so the corresponding exponential-series remainders vanish uniformly as the truncation increases. Taking $n\to\infty$ and then the truncation to infinity proves the [bounded-degree pairing avoidance estimate](../../../../../../bounded-degree-pairing-avoidance-estimate.md) $\Pr(Z=0)=e^{-\Lambda}+o(1)$. This does not require $\lambda$ or $\mu$ to converge. The exponential is bounded away from zero, so the additive error is also a relative $o(1)$ error.

Multiplying by the pairing count and dividing by the representation factor gives

$$
\boxed{|L(\mathbf d;G_0)|\sim e^{-\lambda/2-\lambda^2/4-\mu}\frac{(2m)_m}{2^m\prod_{i=1}^n d_i!}.}
$$

The factor $(2m)_m$ multiplies the exponential; it is not part of its exponent. The TeX aid misgroups this factor, whereas the original PDF is unambiguous. The bounded-degree proof also covers the stated additional assumption $2m-n\to\infty$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
