<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\phi=\phi^1_{p,q}$ and $C_n=\phi(0\leftrightarrow e_n)$. We use these standard facts about the [infinite-volume wired random-cluster measure](../../../../../../infinite-volume-wired-random-cluster-measure.md) for $q\ge1$: it is translation invariant and invariant under coordinate reflections/permutations; it has [positive association of the random-cluster model](../../../../../../positive-association-of-the-random-cluster-model.md); and every conditional edge-open [probability](../../../../../../probability.md) is at least

$$
r=\frac{p}{p+q(1-p)}>0.
$$

The last bound follows because an [edge](../../../../../../edge-of-a-graph.md) either leaves its component count unchanged on opening, giving [probability](../../../../../../probability.md) $p$, or merges two components, giving $p/(p+q(1-p))$. These are standard infinite-volume properties of the limit obtained from the finite wired laws by [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md). [Positive association of random variables](../../../../../../positive-association-of-random-variables.md) applies to connection events by increasing approximation with finite-path events.

Opening the $n$ [edges](../../../../../../edge-of-a-graph.md) of the straight segment gives $C_n\ge r^n$, so its logarithm is finite. The events $A=\{0\leftrightarrow e_m\}$ and $B=\{e_m\leftrightarrow e_{m+n}\}$ are increasing, and their intersection implies connection to $e_{m+n}$. Thus

$$
C_{m+n}\ge\phi(A\cap B)\ge\phi(A)\phi(B)=C_mC_n.
$$

The sequence $a_n=-\log C_n$ is a [subadditive sequence](../../../../../../subadditive-sequence.md), with $0\le a_n\le-n\log r$. Part (a) proves the [random-cluster inverse correlation length](../../../../../../random-cluster-inverse-correlation-length.md) exists and is finite:

$$
\boxed{\alpha(p,q)=\lim_n\frac{a_n}{n}=\inf_n\frac{a_n}{n}\in[0,-\log r].}
$$

Since $a_n/n\ge\alpha$ for every $n$, exponentiating yields the requested bound

$$
\boxed{\phi^1_{p,q}(0\leftrightarrow e_n)\le e^{-n\alpha(p,q)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
