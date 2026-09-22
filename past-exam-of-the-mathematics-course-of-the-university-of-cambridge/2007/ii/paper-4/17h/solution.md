<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

Let $d_v$ be the vertex degrees and let $r_{ij}$ count common neighbours of distinct vertices. Count unoriented length-two paths by their centre or endpoints:

$$
P_2=\sum_v\binom{d_v}{2}=\sum_{i<j}r_{ij}.
$$

If no four-cycle occurs, $r_{ij}\leq1$, so $P_2\leq\binom n2$. By [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), $P_2\geq\frac12[(2m)^2/n-2m]$. Solving $4m^2-2nm\leq n^2(n-1)$ gives

$$
\boxed{m\leq\frac n4(1+\sqrt{4n-3}).}
$$

If $m\geq n(n-1)/4$, the same bound and monotonicity of $2m^2/n-m$ in this range give $P_2\geq n(n-1)(n-3)/8$ (the small $n$ cases are immediate). Every pair of common neighbours supplies a four-cycle, counted twice through its two opposite vertex pairs, so [four-cycle counting by common neighbours](../../../../../four-cycle-counting-by-common-neighbours.md) gives

$$
C_4(G)=\frac12\sum_{i<j}\binom{r_{ij}}2.
$$

Let $N=\binom n2$ and $\bar r=P_2/N\geq(n-3)/4$. Convexity of $r(r-1)/2$ gives $C_4\geq(N/2)\binom{\bar r}2$. For $n\geq7$, this function is increasing on the needed range, giving

$$
\boxed{C_4(G)\geq\frac12\binom n2\binom{(n-3)/4}{2}.}
$$

For $3\leq n\leq6$ the printed right-hand side is nonpositive and the conclusion is trivial. **At $n=2$ the printed cycle bound is false**: a single edge meets the edge hypothesis but has no four-cycles, while the right-hand side is $5/64>0$. Thus this particular bound needs the intended $n\geq3$ restriction; the other counting statements above do not have this defect.

On four chosen vertices there are three distinct cycle subgraphs, each present with probability $2^{-4}$ in the stated random graph. Extra edges do not destroy these subgraphs. Therefore

$$
\boxed{\mathbb EC_4=\frac3{16}\binom n4.}
$$

For positive expectation, [Markov inequality](../../../../../markov-inequality.md) gives

$$
P(C_4\leq(1+2\epsilon)\mathbb EC_4)
\geq1-\frac1{1+2\epsilon}
=\frac{2\epsilon}{1+2\epsilon}\geq\epsilon
$$

when $0<\epsilon<1/2$. If $n<4$, the cycle count is identically zero and the requested event has probability one.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
