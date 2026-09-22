<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $H$ be the $r$-[uniform hypergraph](../../../../../../uniform-hypergraph.md) and use [strong saturation of a uniform hypergraph](../../../../../../strong-saturation-of-a-uniform-hypergraph.md) in its immediate-completion sense: each missing edge $e$ lies in an $(r+t)$-set $T$ whose other $r$-subsets are already edges of $H$. The argument allows existing [hypergraph cliques](../../../../../../complete-uniform-hypergraph.md). Take $n\geq r+t$, the usual parameter range; if $r\leq n<r+t$, strong saturation forces every possible edge to be present, and the inequality is immediate whenever its binomial terms are defined. The case $t=0$ has the trivial lower bound zero.

For $t\geq1$, choose distinct real numbers $z_1,\ldots,z_n$ and form the $t\times n$ [Vandermonde matrix](../../../../../../vandermonde-matrix.md) $M$ whose $i$th column is $(1,z_i,\ldots,z_i^{t-1})^T$. Every $t$ columns are [linearly independent](../../../../../../linear-independence.md) by the [Vandermonde determinant](../../../../../../vandermonde-determinant.md). Set $U=\ker M\subseteq\mathbb R^n$, so $\dim U=n-t$, and work in the [quotient vector space](../../../../../../quotient-vector-space.md)

$$
W=\bigwedge^r\mathbb R^n\big/\bigwedge^rU,\qquad\dim W=\binom nr-\binom{n-t}r.
$$

Here the inclusion of $\bigwedge^rU$ is injective: extend a basis of $U$ to a basis of $\mathbb R^n$ and use the resulting wedge bases of the [exterior powers](../../../../../../exterior-power.md). Write $w_e$ for the image in $W$ of the coordinate wedge indexed by an $r$-set $e$. All these images span $W$.

For any $(r+t)$-set $T$, let $V_T$ be its coordinate subspace. The restriction of $M$ has rank $t$, so $U\cap V_T$ has dimension $r$. Wedge a basis of this intersection to obtain a nonzero element

$$
\omega_T=\sum_{\substack{e\subseteq T\\|e|=r}}c_e\,e_e\in\bigwedge^rU.
$$

Every coefficient $c_e$ is nonzero. Indeed, projection of $U\cap V_T$ onto the $e$ coordinates is an isomorphism: a vector in its kernel is supported on $T\setminus e$, whose $t$ columns of $M$ are independent. The coefficient is the determinant of that projection in the chosen bases. Passing to $W$ therefore gives a [linear dependence](../../../../../../linear-dependence.md)

$$
\sum_{\substack{e\subseteq T\\|e|=r}}c_e w_e=0\qquad(c_e\ne0).
$$

If $e$ is missing from $H$, take its strong-saturation witness $T$. The dependence expresses $w_e$ in the span of the $w_f$ for the other edges $f\subseteq T$, all of which are present. Thus the vectors indexed by the present edges span all of $W$. The [exterior-power quotient bound for strong hypergraph saturation](../../../../../../exterior-power-quotient-bound-for-strong-hypergraph-saturation.md) follows:

$$
\boxed{|E(H)|\geq\dim W=\binom nr-\binom{n-t}r.}
$$

The bound is sharp: include precisely the $r$-sets meeting one fixed $t$-set $S$. A missing edge $e$ is disjoint from $S$, and every other $r$-subset of $e\cup S$ meets $S$, so adding $e$ immediately completes a [hypergraph clique](../../../../../../complete-uniform-hypergraph.md) of order $r+t$. The number of included edges is exactly the displayed bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
