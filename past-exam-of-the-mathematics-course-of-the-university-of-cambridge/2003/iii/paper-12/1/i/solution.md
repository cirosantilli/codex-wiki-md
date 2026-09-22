<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

It suffices to find a [tree component](../../../../../../tree-component.md) of order $k$. Let $X$ count such [graph components](../../../../../../component-graph-theory.md) in the [binomial random graph](../../../../../../binomial-random-graph.md). The [Cayley formula](../../../../../../cayley-s-formula.md) and independent [edges](../../../../../../edge-of-a-graph.md) give the [tree-component expectation in the Erdős-Rényi model](../../../../../../tree-component-expectation-in-the-erdos-renyi-model.md)

$$
\mu=\mathbb EX=\binom nk k^{k-2}p^{k-1}(1-p)^{k(n-k)+\binom k2-k+1}.
$$

Here $k$ is fixed. The upper bound on $p$ implies $p=O(\log n/n)$, hence $np^2=o(1)$ and

$$
\mu\sim\frac{k^{k-2}}{k!}n^kp^{k-1}e^{-knp}=\frac{k^{k-2}}{k!}n(np)^{k-1}e^{-knp}.
$$

We first verify that this [expected value](../../../../../../expected-value.md) diverges throughout the permitted interval, including when $\omega$ grows quickly. If $np\leq1$, the exponential factor is at least $e^{-k}$ and $n^kp^{k-1}\geq\omega^{k-1}$. If $1\leq np\leq(\log n)/(2k)$, then $n(np)^{k-1}e^{-knp}\geq\sqrt n$. Finally, if $np\geq(\log n)/(2k)$, the upper bound on $p$ gives

$$
e^{-knp}\geq\frac{e^\omega}{n(\log n)^{k-1}},\qquad n(np)^{k-1}e^{-knp}\geq\frac{e^\omega}{(2k)^{k-1}}.
$$

Thus $\mu\to\infty$ in all three cases.

For distinct $k$-element [vertex sets](../../../../../../vertex-set.md) $S,T$, write $I_S,I_T$ for their tree-component indicators. If they overlap, they cannot both be distinct [connected components of a graph](../../../../../../component-graph-theory.md), so $\mathbb E(I_SI_T)=0$. If they are disjoint, the absent [edges](../../../../../../edge-of-a-graph.md) between the two sets are counted twice in the product of their marginal probabilities and once in the joint probability. Therefore

$$
\mathbb E(I_SI_T)=(1-p)^{-k^2}\mathbb EI_S\,\mathbb EI_T.
$$

Summing and discarding the negative overlap contributions yields

$$
\operatorname{Var}X\leq\mu+\mu^2\bigl((1-p)^{-k^2}-1\bigr),\qquad \frac{\operatorname{Var}X}{\mu^2}\leq\frac1\mu+O(p)\longrightarrow0.
$$

The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) now gives $\Pr(X=0)\leq\operatorname{Var}X/\mu^2\to0$. Consequently **there is a component of order $k$ with high probability**, in fact a [tree component](../../../../../../tree-component.md). The argument proves the entire [fixed-order tree-component window](../../../../../../fixed-order-tree-component-window.md), rather than only a particular choice of $p$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
