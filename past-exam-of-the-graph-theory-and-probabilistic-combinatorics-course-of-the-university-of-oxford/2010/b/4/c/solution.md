<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [threshold function](../../../../../threshold-function-for-a-monotone-graph-property.md) $p^*(n)$ has the following meaning: if $p/p^*\to0$, the [probability](../../../../../probability.md) of a $K_5$ tends to zero; if $p/p^*\to\infty$, that [probability](../../../../../probability.md) tends to one. Behavior at a fixed constant multiple is not specified by this definition.

Let $X$ count the five-[vertex](../../../../../vertex-graph-theory.md) subsets spanning $K_5$ in the [Erdős-Rényi model](../../../../../erdos-renyi-model.md) $G(n,p)$. Then

$$
\mu=\mathbb EX=\binom n5p^{10}.
$$

If $p\ll n^{-1/2}$, then $\mu\to0$, so [Markov inequality](../../../../../markov-s-inequality.md) gives $P(X>0)\leq\mu\to0$.

Now let $p=n^{-1/2}w$ with $w\to\infty$. Then $\mu\sim w^{10}/120\to\infty$. Distinct copies have dependent indicators only if their [vertex](../../../../../vertex-graph-theory.md) sets share at least two vertices. If they share $j\in\{2,3,4\}$ vertices, they share $\binom j2$ edges; there are $O(n^{10-j})$ ordered such pairs, and their joint [probability](../../../../../probability.md) is $p^{20-\binom j2}$. Consequently

$$
\frac\Delta{\mu^2}
=O\left(\frac1{n^2p}+\frac1{n^3p^3}+\frac1{n^4p^6}\right)
=O\left(\frac1{n^{3/2}w}+\frac1{n^{3/2}w^3}+\frac1{nw^6}\right)\longrightarrow0.
$$

Part (b) gives $P(X=0)\to0$. Therefore

$$
\boxed{p^*(n)=n^{-1/2}.}
$$

This is the five-[vertex](../../../../../vertex-graph-theory.md) instance of the [fixed-size clique appearance threshold](../../../../../fixed-size-clique-appearance-threshold.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
