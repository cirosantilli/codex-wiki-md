<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Ramsey's theorem](../../../../../../ramsey-s-theorem.md) for $r$-sets says that every [finite coloring](../../../../../../finite-coloring.md) of $[\mathbb N]^{(r)}$ has an infinite [monochromatic set](../../../../../../monochromatic-set.md). We prove it by [mathematical induction](../../../../../../mathematical-induction.md) on $r$. The case $r=1$ is the [infinite pigeonhole principle](../../../../../../infinite-pigeonhole-principle.md). Suppose the result holds for $r-1$, and let $c:[\mathbb N]^{(r)}\to[k]$. Choose $a_1$, then use the induction hypothesis on the coloring $F\mapsto c(F\cup\{a_1\})$ to obtain an infinite set $M_1$ on which this color is constant, say $d_1$. Inductively choose

$$
a_j\in M_{j-1},\qquad
M_j\subseteq M_{j-1}\setminus\{a_j\}
$$

so that $c(F\cup\{a_j\})=d_j$ for every $F\in[M_j]^{(r-1)}$. Some color $d$ occurs for infinitely many $d_j$. If $j_1<j_2<\cdots$ are the corresponding indices, every $r$-set from $\{a_{j_1},a_{j_2},\ldots\}$ has color $d$: take its least-indexed element $a_{j_s}$, after which its other $r-1$ elements lie in $M_{j_s}$. This proves the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
