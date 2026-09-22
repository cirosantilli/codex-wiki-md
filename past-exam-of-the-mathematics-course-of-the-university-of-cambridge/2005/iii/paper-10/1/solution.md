<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Identify the [discrete cube](../../../../../boolean-hypercube.md) $Q_n$ with the subsets of $[n]$, with [hypercube graph](../../../../../hypercube-graph.md) adjacency given by changing one element. Write $N[A]$ for the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) and $\partial A=N[A]\setminus A$ for the [external vertex boundary](../../../../../external-vertex-boundary.md). The [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md) first orders by set size and then by [lexicographic order](../../../../../lexicographic-order.md), with the smallest differing coordinate belonging to the earlier set.

[Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) states that, for every [set family](../../../../../set-family.md) $A\subseteq Q_n$,

$$
|N[A]|\geq |N[C(|A|)]|,
\qquad\text{equivalently}\qquad
|\partial A|\geq|\partial C(|A|)|.
$$

Here is the [simplicial section compression](../../../../../simplicial-section-compression.md) proof. Induct on $n$, the one-dimensional case being immediate. Split $A$ by a coordinate into sections $A_0,A_1\subseteq Q_{n-1}$. Its neighbourhood sections are

$$
N[A]_0=N[A_0]\cup A_1,\qquad N[A]_1=N[A_1]\cup A_0.
$$

Replace $A_0,A_1$ by equally large simplicial [initial segments](../../../../../initial-segment.md) $I_0,I_1$. By induction $|N[I_j]|\leq|N[A_j]|$. Also the neighbourhood of a simplicial [initial segment](../../../../../initial-segment.md) is itself a simplicial [initial segment](../../../../../initial-segment.md): at its last occupied level the extra vertices form the [upper shadow](../../../../../upper-shadow.md) of a lexicographic [initial segment](../../../../../initial-segment.md), again lexicographically initial. Consequently the compressed unions have sizes $\max\{|N[I_0]|,|I_1|\}$ and $\max\{|N[I_1]|,|I_0|\}$, no larger than the original unions. The compression preserves $|A|$ and cannot increase $|N[A]|$.

Repeat in every coordinate until all sections are initial. Every nontrivial compression strictly decreases the sum of the global simplicial positions, so the process terminates. To describe the [terminal families for simplicial section compression](../../../../../terminal-families-for-simplicial-section-compression.md), suppose an earlier absent vertex $S$ precedes a later present vertex $T$. They cannot share a coordinate value: otherwise they lie in the same compressed section, contradicting its initiality. Thus $T=[n]\setminus S$. No vertex can lie strictly between them in the order, since it would make another absent/present pair that is not complementary. Hence the terminal family is either $C(|A|)$ or that segment with its last vertex $S$ exchanged for its immediate complementary successor $T$.

For odd $n=2m+1$, that exceptional exchange crosses the middle levels: $S=\{m+2,\ldots,2m+1\}$ and $T=\{1,\ldots,m+1\}$. For $m\geq1$, all sets of size at most $m+1$ remain in the neighbourhood after the exchange, since an $(m+1)$-set has at least two lower neighbours and only one was removed. The new $T$ can only add vertices of size $m+2$.

For even $n=2m$, the only consecutive complementary pair in one level is $S=\{1,m+2,\ldots,2m\}$ and $T=\{2,\ldots,m+1\}$. The original segment contains all sets below size $m$ and all $m$-sets containing 1. For $m\geq2$, its neighbourhood contains all sets of size at most $m$ and all $(m+1)$-sets containing 1; every such upper set still has an included lower neighbour after the single removal. The new $T$ can only add further neighbours. The cases $n=1,2$ follow directly, with the exceptional families related to the initial ones by a [graph automorphism](../../../../../graph-automorphism.md). Thus neither exception improves the neighbourhood, completing the induction.

For the [half-cube vertex-boundary extrema](../../../../../half-cube-vertex-boundary-extrema.md), if $n=2m+1$, the initial half cube is all sets of size at most $m$; its boundary is the next level, of size $\binom{2m+1}{m+1}$. If $n=2m$, it contains all levels below $m$ and the $m$-sets containing 1. The boundary consists of the $m$-sets avoiding 1 and the $(m+1)$-sets containing 1, giving $2\binom{2m-1}{m}=\binom{2m}{m}$.

No boundary can exceed the $2^{n-1}$ vertices outside a half cube. Taking all vertices of even [Hamming weight](../../../../../hamming-weight.md) attains that bound, because every odd-weight vertex is adjacent to one of them. Therefore, for $n\geq1$,

$$
\boxed{\min_{|A|=2^{n-1}}|\partial A|=\binom n{\lfloor n/2\rfloor},\qquad
\max_{|A|=2^{n-1}}|\partial A|=2^{n-1}}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
