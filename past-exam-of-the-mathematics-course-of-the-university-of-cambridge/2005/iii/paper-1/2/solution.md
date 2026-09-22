<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

First prove [Simplicity of alternating groups](../../../../../simplicity-of-alternating-groups.md). The $3$-cycles generate $A_n$: express an even permutation as an even number of [transpositions](../../../../../transposition-permutation.md) and pair them. A pair sharing a point is a $3$-cycle, an identical pair cancels, and a disjoint pair can be written $(ab)(cd)=(acb)(acd)$. All $3$-cycles are conjugate in $A_n$ when $n\ge5$: a conjugator in $S_n$ can have its parity corrected by a [transposition](../../../../../transposition-permutation.md) on two points outside the target triple, without changing its effect on that triple.

Let $1\ne N\triangleleft A_n$ and choose $1\ne\sigma\in N$. Some $3$-cycle $\tau$ does not commute with $\sigma$. Indeed, commuting with every $3$-cycle would preserve every triple setwise; intersecting all triples containing a given point forces that point to be fixed, so would make $\sigma=1$. The nonidentity [group commutator](../../../../../group-commutator.md) $\sigma\tau\sigma^{-1}\tau^{-1}\in N$ is supported on at most six points. Its possible nontrivial even cycle types are a $3$-cycle, a double [transposition](../../../../../transposition-permutation.md), a $5$-cycle, two disjoint $3$-cycles, or a $4$-cycle times a [transposition](../../../../../transposition-permutation.md). Each yields a $3$-cycle in $N$ by explicit [group commutators](../../../../../group-commutator.md):

For $(ab)(cd)$, use $\tau=(cde)$ with a fifth point $e$; [conjugation](../../../../../conjugation.md) reverses $\tau$, so the [group commutator](../../../../../group-commutator.md) is $\tau^{-2}=\tau$. For $(abcde)$, use $(abc)$: the [group commutator](../../../../../group-commutator.md) is $(bcd)(abc)^{-1}=(adb)$. The same calculation works for $(abcd)(ef)$. For $(abc)(def)$, use $(abd)$; its conjugate is $(bce)$, and the product $(bce)(abd)^{-1}$ is a $5$-cycle, reducing to the preceding case. Thus $N$ contains a $3$-cycle, hence the whole [conjugacy class](../../../../../conjugacy-class.md) of $3$-cycles, and hence all of $A_n$. Therefore

$$
\boxed{A_n\text{ is simple for }n\ge5.}
$$

For the exceptional [automorphism](../../../../../automorphism.md), a [duad](../../../../../duad.md) is an unordered pair of six points, a [syntheme](../../../../../syntheme.md) is a partition into three duads, and a [pentad](../../../../../total-of-synthemes.md) is a set of five synthemes covering every duad once. There are fifteen synthemes. To count pentads, fix $12|34|56$, where bars separate duads. A syntheme disjoint from it in duads is one of eight; the union of the two matchings is a six-cycle, so the [stabilizer](../../../../../stabilizer-subgroup.md) of the fixed syntheme is transitive on these eight choices. For the choice $13|25|46$, the remaining compatible synthemes are $14|26|35$, $15|24|36$, $16|23|45$ and $16|24|35$. The last shares a duad with each of the first three and cannot belong to a completion; the first three form the unique completion. Thus each of the eight choices has a unique completion through the fixed syntheme. Each completion contains four of them, so exactly two pentads contain a fixed syntheme, and there are $15\cdot2/5=6$ pentads in total.

Here is the complete list, which also defines concrete labels for the induced action:

$$
\begin{array}{c|l}
1&12|34|56,\ 13|25|46,\ 14|26|35,\ 15|24|36,\ 16|23|45\\
2&12|34|56,\ 13|26|45,\ 14|25|36,\ 15|23|46,\ 16|24|35\\
3&12|35|46,\ 13|24|56,\ 14|25|36,\ 15|26|34,\ 16|23|45\\
4&12|35|46,\ 13|26|45,\ 14|23|56,\ 15|24|36,\ 16|25|34\\
5&12|36|45,\ 13|24|56,\ 14|26|35,\ 15|23|46,\ 16|25|34\\
6&12|36|45,\ 13|25|46,\ 14|23|56,\ 15|26|34,\ 16|24|35
\end{array}
$$

Relabelling points gives a [group homomorphism](../../../../../group-homomorphism.md) $\Phi:S_6\to S_6$ on these pentads. Direct substitution in the table gives

$$
\Phi((12))=(12)(34)(56),\qquad
\Phi((123))=(145)(263).
$$

The restriction to $A_6$ is nontrivial, hence faithful by the simplicity just proved. Therefore the full kernel has order at most two. An order-two [normal subgroup](../../../../../normal-subgroup.md) would be central, whereas $S_6$ has trivial centre: an element centralizing every [transposition](../../../../../transposition-permutation.md) fixes every unordered pair and consequently every point. The kernel is trivial, and equal orders make $\Phi$ an [automorphism](../../../../../automorphism.md). It preserves $A_6$, because that is the unique index-two subgroup of $S_6$: any nontrivial [group homomorphism](../../../../../group-homomorphism.md) to $C_2$ sends every conjugate [transposition](../../../../../transposition-permutation.md) to the nonidentity element, and is therefore the sign map. Its restriction is the [pentad construction of the exceptional alternating-group automorphism](../../../../../pentad-construction-of-the-exceptional-alternating-group-automorphism.md). It maps a $3$-cycle to two disjoint $3$-cycles, while [conjugation](../../../../../conjugation.md) in $S_6$ preserves [cycle type](../../../../../cycle-type.md). Hence **this [automorphism](../../../../../automorphism.md) of $A_6$ is not induced by any element of $S_6$**.

For the other degrees, recover the points from $3$-cycles. An element of order three has type $3^k1^{n-3k}$. Its [centralizer](../../../../../centralizer.md) in $S_n$ has order $3^k k!(n-3k)!$. That [centralizer](../../../../../centralizer.md) contains an odd permutation: either swap two fixed points, or, when $k\ge2$, swap two three-cycles by three [transpositions](../../../../../transposition-permutation.md). Thus

$$
|C_{A_n}(x)|=\frac{3^k k!(n-3k)!}{2}.
$$

For $n=5$, only $k=1$ is possible. For $n\ge7$, the $k=1$ value is strictly largest. For $k=2$ equality first occurs at $n=6$, and the ratio increases strictly with $n$. For $k\ge3$, already at $n=3k$ one has $(3k-3)!>3^{k-1}k!$: it holds at $k=3$, and the inductive ratio is $(3k)(3k-1)(3k-2)>3(k+1)$. Increasing $n$ again increases the ratio. Consequently every [automorphism](../../../../../automorphism.md) preserves the set of $3$-cycles when $n\ne6$.

Each [cyclic subgroup](../../../../../cyclic-subgroup.md) generated by a $3$-cycle corresponds to its three-point support. Two distinct such subgroups commute exactly when the supports are disjoint. If they meet in one point, products of their nonidentity generators have order five. If they meet in two points, those products have order two or three. These intrinsic tests recover adjacency in the [Johnson graph](../../../../../johnson-graph.md) $J(n,3)$, so the [automorphism](../../../../../automorphism.md) acts on its vertices.

We can reconstruct the underlying points without an additional group-theoretic bound. The [maximal cliques of a Johnson graph](../../../../../maximal-cliques-of-a-johnson-graph.md) in $J(n,3)$ are the $n-2$ triples containing a fixed pair, and the four triples contained in a fixed four-set. To verify the classification, take adjacent triples $D\cup\{a\}$ and $D\cup\{b\}$ with $|D|=2$. Any common adjacent triple either contains $D$ or lies in $D\cup\{a,b\}$. A triple of the first kind outside that four-set is not adjacent to a triple of the second kind omitting a point of $D$, so a clique cannot mix the two alternatives. Extending a clique therefore gives exactly one of the two listed families.

For $n\ge5$, $n\ne6$, their sizes distinguish the pair-containing cliques. Their intersections reconstruct the pair graph $J(n,2)$: two such cliques intersect precisely when their defining pairs meet in one point. In this graph the maximal cliques are stars of $n-1$ pairs through a point and triangles of three pairs within a triple. These sizes are different for $n\ge5$, so its [automorphisms](../../../../../automorphism.md) permute the stars and hence the points. Every pair is the intersection of its two point stars, and every triple is determined by its three pairs. Thus the original graph action comes from some $\pi\in S_n$.

Undo [conjugation](../../../../../conjugation.md) by $\pi$. The remaining [group automorphism](../../../../../group-automorphism.md) $\beta$ fixes each cyclic $3$-subgroup, so it fixes or inverts each generator. For adjacent supports, inverting exactly one generator changes the order of their product between two and three; inverting both preserves that order. Hence the two inversion choices must agree. The triple-support graph is connected, since one can replace differing points one at a time, so the choice is uniform. Inverting every $3$-cycle is impossible: take $c=(123)$, $d=(142)$, whose product is the $3$-cycle $(143)$. Then $\beta(cd)=(cd)^{-1}=d^{-1}c^{-1}$, whereas the [group homomorphism](../../../../../group-homomorphism.md) property would give $c^{-1}d^{-1}$; these are unequal because $c,d$ do not commute. Therefore $\beta$ fixes every $3$-cycle and is the identity. Conversely, [conjugation](../../../../../conjugation.md) by $S_n$ acts faithfully on $A_n$, since centralizing all $3$-cycles fixes every triple and every point. The [automorphisms of alternating groups from triple supports](../../../../../automorphisms-of-alternating-groups-from-triple-supports.md) are exactly

$$
\boxed{\operatorname{Aut}(A_n)\cong S_n\qquad(n\ge5,\ n\ne6).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
