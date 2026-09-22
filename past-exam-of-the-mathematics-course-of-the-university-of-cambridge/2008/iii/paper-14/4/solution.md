<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $U=G\sqcup\bar G$, with the two copies of the [graph vertex](../../../../../vertex-graph-theory.md) [set](../../../../../set-split.md) distinguished. In $G\boxtimes\bar G$, the diagonal pairs $(v,v)$ form an [independent set](../../../../../independent-set-graph-theory.md) of size $n$: for $v\ne w$, their adjacency cannot hold in both a [graph](../../../../../graph-split.md) and its [complement graph](../../../../../complement-graph.md). There is another such diagonal [set](../../../../../set-split.md) in $\bar G\boxtimes G$. These two types lie in different components of $U^{\boxtimes2}$, so their [set union](../../../../../set-union.md) is independent. Thus

$$
\alpha(U^{\boxtimes2})\ge2n,\qquad\boxed{c(U)\ge\sqrt{2n},}
$$

which proves the printed bound.

A stronger [complement-pair capacity gain](../../../../../complement-pair-capacity-gain.md) will make the strict inequality transparent. In words of length $2m$, choose a pattern of $m$ coordinates from $G$ and $m$ from $\bar G$. Match the $i$th coordinate of the first type with the $i$th of the second type, and put the same [graph vertex](../../../../../vertex-graph-theory.md) label in each pair. This gives $n^m$ independent words for each pattern: if two label tuples differ, their differing pair has a nonedge in one of the two complementary [graphs](../../../../../graph-split.md). Codes belonging to distinct patterns are mutually nonadjacent, since some coordinate lies in different components of the disjoint [set union](../../../../../set-union.md). Consequently

$$
\alpha(U^{\boxtimes2m})\ge\binom{2m}m n^m.
$$

The inequalities $4^m/(2m+1)\le\binom{2m}m\le4^m$ show that its $2m$th root tends to two. Therefore

$$
\boxed{c(G\sqcup\bar G)\ge2\sqrt n.}
$$

This strengthens, rather than changes, the bound requested in the PDF.

For a [polynomial representation of a graph](../../../../../polynomial-representation-of-a-graph.md) over a [field](../../../../../field.md) $F$, choose points $a_v\in F^r$ and [polynomials](../../../../../polynomial-split.md) $f_v\in M$, where $M\subseteq F[z_1,\ldots,z_r]$ is a finite-dimensional [vector](../../../../../vector.md) space, such that

$$
f_v(a_v)\ne0,\qquad f_v(a_w)=0\quad\text{whenever }v\ne w\text{ are nonadjacent}.
$$

No condition is imposed at adjacent pairs. To bound a [strong power](../../../../../strong-graph-power.md), put its [polynomials](../../../../../polynomial-split.md) in disjoint variable blocks:

$$
F_{(v_1,\ldots,v_m)}(z^{(1)},\ldots,z^{(m)})
=\prod_{i=1}^m f_{v_i}(z^{(i)}).
$$

They lie in a [polynomial](../../../../../polynomial-split.md) space canonically identified with $M^{\otimes m}$, of [dimension](../../../../../dimension-vector-space.md) $(\dim_F M)^m$. For an [independent set](../../../../../independent-set-graph-theory.md) of words, evaluation of their [polynomials](../../../../../polynomial-split.md) at their associated point tuples is a diagonal matrix with nonzero diagonal: distinct words have a nonedge coordinate, which supplies a zero factor. The [polynomials](../../../../../polynomial-split.md) in that [independent set](../../../../../independent-set-graph-theory.md) are therefore linearly independent, since evaluating any linear relation at each tuple forces its corresponding coefficient to be zero. Hence

$$
\alpha(G^{\boxtimes m})\le(\dim_F M)^m,
\qquad\boxed{c(G)\le\dim_F M.}
$$

This is the [polynomial](../../../../../polynomial-split.md) form of the [Haemers rank bound](../../../../../haemers-rank-bound.md), proved here by evaluations and [tensor products](../../../../../tensor-product.md) rather than assumed.

For an explicit counterexample, let the [graph vertices](../../../../../vertex-graph-theory.md) of $G$ be the five-element [subsets](../../../../../subset.md) of $[20]$. Join distinct $A,B$ exactly when $|A\cap B|$ is odd. There are $n=\binom{20}5=15504$ [graph vertices](../../../../../vertex-graph-theory.md). Over $\mathbb F_2$, take $a_B=\mathbf1_B$ and

$$
f_A(z)=\sum_{i\in A}z_i.
$$

At the diagonal $f_A(a_A)=5=1$ in the [field](../../../../../field.md). At a distinct nonedge the [set intersection](../../../../../set-intersection.md) is even, so $f_A(a_B)=0$. These [polynomials](../../../../../polynomial-split.md) lie in the twenty-dimensional space spanned by $z_1,\ldots,z_{20}$, proving **$c(G)\le20$**.

Represent the [complement graph](../../../../../complement-graph.md) over $\mathbb F_3$, using the same [indicator vectors](../../../../../indicator-vector.md) and

$$
g_A(z)=\sum_{\{i,j\}\subseteq A}z_iz_j.
$$

Its evaluation at $a_B$ is $\binom{|A\cap B|}2$. The diagonal value is $\binom52=10=1$ modulo three. Distinct nonedges of $\bar G$ are edges of $G$, so the [set intersection](../../../../../set-intersection.md) size is one or three. Their evaluations are respectively zero and $\binom32=3=0$ modulo three. The [polynomials](../../../../../polynomial-split.md) belong to the space spanned by the squarefree quadratic monomials $z_iz_j$, $i<j$, of [dimension](../../../../../dimension-vector-space.md) $\binom{20}2=190$. Therefore **$c(\bar G)\le190$**.

The [graph capacity](../../../../../shannon-capacity-of-a-graph.md) inequalities are real-number bounds regardless of which [field](../../../../../field.md) supplies the [polynomial representation of a graph](../../../../../polynomial-representation-of-a-graph.md). Combining them with the stronger [set union](../../../../../set-union.md) lower bound gives

$$
\boxed{c(G\sqcup\bar G)\ge2\sqrt{15504}>210\ge c(G)+c(\bar G),}
$$

since $4\cdot15504=62016>210^2=44100$. This proves [nonadditivity of Shannon capacity](../../../../../nonadditivity-of-shannon-capacity.md) for the [graph](../../../../../graph-split.md) just defined, with both individual upper bounds calculated explicitly.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
