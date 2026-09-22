<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the Erdős-Rado selection argument. Put

$$
m=R^{(2)}(k-1)+1.
$$

Starting with a sufficiently large reservoir, choose vertices $v_1,\ldots,v_m$ in order. After choosing $v_j$, successively halve the remaining reservoir for each $i<j$ so that the colour of

$$
\{v_i,v_j,x\}
$$

is constant as $x$ ranges over the final reservoir. The total number of halvings is at most $\binom m2$, so $2^{\binom m2}+m$ initial vertices suffice.

Colour the pair $ij$, for $i<j<m$, by the stabilized colour of $\{v_i,v_j,v_\ell\}$ for $\ell>j$. Among $v_1,\ldots,v_{m-1}$, the definition of $R^{(2)}(k-1)$ gives a monochromatic set of $k-1$ vertices. Adjoining $v_m$ gives a monochromatic $k$-set for the original triple colouring. Hence

$$
R^{(3)}(k)\le2^{\binom{R^{(2)}(k-1)+1}{2}}+R^{(2)}(k-1)+1.
$$

The [binomial upper bound for a Ramsey number](../../../../../../binomial-upper-bound-for-a-ramsey-number.md) gives $R^{(2)}(k-1)<2^{2k}$, so the right-hand side is at most

$$
\boxed{2^{2^{Ck}}}
$$

for an absolute $C>0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
