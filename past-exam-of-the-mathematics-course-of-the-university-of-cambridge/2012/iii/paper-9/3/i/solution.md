<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $0<\lambda=1-\varepsilon<1$, as required for this nontrivial subcritical [binomial random graph](../../../../../../binomial-random-graph.md). Put $\delta=\lambda-1-\log\lambda>0$. A [breadth-first exploration of a binomial random graph](../../../../../../breadth-first-exploration-of-a-binomial-random-graph.md) is dominated by a [Galton-Watson process](../../../../../../galton-watson-process.md) whose offspring counts are [independent random variables](../../../../../../independent-random-variables.md) with law $\operatorname{Bin}(n,\lambda/n)$. If its [total progeny](../../../../../../total-progeny-of-a-branching-process.md) $T$ is at least $j$, the first $j-1$ offspring counts sum to at least $j-1$. Their [moment-generating function](../../../../../../moment-generating-function.md) is bounded by that of a [Poisson distribution](../../../../../../poisson-distribution.md) of mean $\lambda(j-1)$. The exponential [Markov inequality](../../../../../../markov-inequality.md), optimized at $t=-\log\lambda$, yields

$$
\mathbb P(T\geq j)\leq e^{-\delta(j-1)}.
$$

Taking $j=\lceil(1+\eta)\log n/\delta\rceil$ for any fixed $\eta>0$, a [union bound](../../../../../../boole-s-inequality.md) over all starting [vertices](../../../../../../vertex-graph-theory.md) gives $\mathbb P(L_1\geq j)=o(1)$.

For the matching lower bound, let $X_j$ count [tree components](../../../../../../tree-component.md) of order $j$. The [tree-component expectation in the Erdős-Rényi model](../../../../../../tree-component-expectation-in-the-erdos-renyi-model.md) is exactly

$$
\mathbb EX_j=\binom nj j^{j-2}p^{j-1}(1-p)^{j(n-j)+\binom j2-j+1}.
$$

For $j=O(\log n)$, the [Stirling formula](../../../../../../stirling-formula.md) gives

$$
\mathbb EX_j=(1+o(1))\frac{n}{\lambda\sqrt{2\pi}\,j^{5/2}}e^{-\delta j}.
$$

Choose $j=\lfloor(1-\eta)\log n/\delta\rfloor$, with $0<\eta<1$. Then $\mathbb EX_j\to\infty$. Distinct overlapping vertex sets cannot both be [graph components](../../../../../../component-graph-theory.md). For disjoint sets, the joint [probability](../../../../../../probability.md) differs from the product only because the $j^2$ between-set [edges](../../../../../../edge-of-a-graph.md) were counted twice as absent. Thus

$$
\frac{\mathbb E[X_j(X_j-1)]}{(\mathbb EX_j)^2}
=\frac{\binom{n-j}j}{\binom nj}(1-p)^{-j^2}
=1+O(j^2/n).
$$

It follows that $\operatorname{var}X_j/(\mathbb EX_j)^2=o(1)$. The [second moment method](../../../../../../second-moment-method.md) gives $X_j>0$ [with high probability](../../../../../../with-high-probability.md). Combining both bounds, and then taking arbitrarily small fixed $\eta$, proves the [sharp subcritical largest-component scale](../../../../../../sharp-subcritical-largest-component-scale.md)

$$
\boxed{L_1=(1+o(1))\frac{\log n}{\delta}=(1+o(1))\ell_0\quad\text{with high probability}.}
$$

Finally the [Taylor expansion](../../../../../../taylor-expansion.md) of $-\log(1-\varepsilon)$ gives $\delta=\varepsilon^2/2+\varepsilon^3/3+\cdots$. The endpoint $\lambda=0$ has no [edges](../../../../../../edge-of-a-graph.md) and is excluded from this logarithmic asymptotic.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
