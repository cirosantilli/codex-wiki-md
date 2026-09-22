<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the single-edge [heat-bath Markov chain](../../../../../../heat-bath-markov-chain.md): choose an edge uniformly and resample it from its conditional random-cluster law. If its endpoints are already connected without that edge, its conditional open probability is $p$; otherwise opening it merges two components and the probability is

$$
\frac p{p+2(1-p)}=\frac p{2-p}.
$$

Detailed balance makes $\phi_{p,2}$ stationary. Driving this chain and Bernoulli heat-bath chains by the same update edges and uniforms gives the stochastic domination

$$
\boxed{\operatorname{Ber}\left(\frac p{2-p}\right)^{\otimes E}
\preceq\phi_{p,2}\preceq
\operatorname{Ber}(p)^{\otimes E}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
