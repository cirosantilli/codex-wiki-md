<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Throughout this question the [binomial random graph](../../../../../../binomial-random-graph.md) has $p=1/2$, as fixed in the introduction. Let $L=\log_2n$ and $s=\lceil2L\rceil$. Count the $s$-vertex [independent sets](../../../../../../independent-set-graph-theory.md) by a [random variable](../../../../../../random-variable-split.md) $I_s$. [Linearity of expectation](../../../../../../linearity-of-expectation.md) gives

$$
\mathbb EI_s=\binom ns2^{-\binom s2}
\leq\frac{n^s2^{-s(s-1)/2}}{s!}
\leq\frac{\sqrt2\,n}{s!}=o(1).
$$

For the second inequality, $s\geq2L$ implies $sL-s(s-1)/2\leq s/2\leq L+1/2$. For the limit, $s!\geq(s/2)^{\lfloor s/2\rfloor}$ grows faster than $n$. By the [first moment method](../../../../../../first-moment-method.md), [with high probability](../../../../../../with-high-probability.md) there is no such [independent set](../../../../../../independent-set-graph-theory.md); any larger [independent set](../../../../../../independent-set-graph-theory.md) would contain one. Thus the [independence number](../../../../../../independence-number.md) satisfies $\alpha(G)\leq s-1<2L$ [with high probability](../../../../../../with-high-probability.md).

Every class of a proper [graph coloring](../../../../../../graph-coloring.md) is an [independent set](../../../../../../independent-set-graph-theory.md), giving **the claimed chromatic lower bound**:

$$
\boxed{\chi(G)\geq\frac n{\alpha(G)}\geq\frac n{2\log_2n}\quad\text{with high probability}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
