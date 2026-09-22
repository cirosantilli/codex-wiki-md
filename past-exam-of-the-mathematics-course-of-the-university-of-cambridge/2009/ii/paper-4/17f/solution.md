<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

For each vertex triple $S$, let $I_S$ indicate that its three edges are present. Then $X=\sum_SI_S$ and

$$
\boxed{\mathbb EX=\binom n3p^3.}
$$

Each [variance](../../../../../variance-split.md) is $p^3(1-p^3)$. Two distinct triples have independent indicators unless they share an edge; in that case their [covariance](../../../../../covariance.md) is $p^5-p^6$. There are $\binom n2\binom{n-2}2=6\binom n4$ unordered pairs sharing an edge. Therefore the [triangle count in a binomial random graph](../../../../../triangle-count-in-a-binomial-random-graph.md) has

$$
\boxed{\operatorname{Var}X=\binom n3p^3(1-p^3)+12\binom n4p^5(1-p).}
$$

If $np\to0$, [Markov inequality](../../../../../markov-inequality.md) gives $\Pr(X>0)\le\mathbb EX\to0$. If $np\to\infty$, then $\mathbb EX\to\infty$ and

$$
\frac{\operatorname{Var}X}{(\mathbb EX)^2}
\le\frac1{\mathbb EX}+O\!\left(\frac1{n^2p}\right)\longrightarrow0.
$$

The second term tends to zero since $n^2p=n(np)\to\infty$. [Chebyshev inequality](../../../../../chebyshev-inequality.md) now gives $\Pr(X=0)\le\operatorname{Var}X/(\mathbb EX)^2\to0$, proving the stated threshold. Here the random-graph phrase “almost surely” means asymptotically almost surely, that is, with probability tending to one.

At $p=n^{-1/2}$, let $Y$ count edges. Direct subtraction gives

$$
\mathbb E(Y-X)=\frac{n(n-1)}{2\sqrt n}-\frac{n(n-1)(n-2)}{6n^{3/2}}
=\frac{n^2-1}{3\sqrt n}\ge\frac16n^{3/2}\quad(n\ge3).
$$

Some graph has $Y-X$ at least this expectation. Successively deleting one edge from each remaining triangle destroys all triangles with at most $X$ deletions, so a [triangle-free graph](../../../../../triangle-free-graph.md) remains with at least $Y-X$ edges. This [triangle deletion in the alteration method](../../../../../triangle-deletion-in-the-alteration-method.md) proves the requested existence bound.

It is **not within a constant factor of the optimum**. A balanced complete bipartite graph has $\lfloor n^2/4\rfloor$ edges and no triangle. Conversely, in a [triangle-free graph](../../../../../triangle-free-graph.md) each edge $uv$ satisfies $d(u)+d(v)\le n$. Summing over edges gives $\sum_vd(v)^2\le nM$, where $M$ is its edge count. [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $4M^2/n\le\sum d(v)^2$, hence $M\le n^2/4$. The optimum is therefore $\boxed{\lfloor n^2/4\rfloor}$, quadratic rather than the obtained $n^{3/2}$ bound.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
