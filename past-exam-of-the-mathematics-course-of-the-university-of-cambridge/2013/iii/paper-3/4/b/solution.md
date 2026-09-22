<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $T_a=\Theta(a)$ for the total of $H'$ assigned to a point $a\in H$. The [duad-syntheme duality on six points](../../../../../../duad-syntheme-duality-on-six-points.md) is constructed entirely from incidence, as follows.

For a [duad](../../../../../../duad.md) $d=\{a,b\}$, define $\Theta(d)$ to be the unique [syntheme](../../../../../../syntheme.md) common to $T_a$ and $T_b$. This is a bijection between the fifteen [duads](../../../../../../duad.md) and the fifteen [synthemes](../../../../../../syntheme.md) of $H'$, by the last incidence count in part (a).

For a [duad](../../../../../../duad.md) $d'$ of $H'$, the three [synthemes](../../../../../../syntheme.md) containing $d'$ each belong to two totals. Each total contains exactly one of these [synthemes](../../../../../../syntheme.md), since its five matchings cover every [duad](../../../../../../duad.md) exactly once. Their three pairs of totals therefore partition all six totals. Pulling these pairs back to $H$ gives a [syntheme](../../../../../../syntheme.md) $s$. Different $d'$ give different $s$, since two distinct [synthemes](../../../../../../syntheme.md) of $H'$ containing $d'$ have intersection exactly that [duad](../../../../../../duad.md). There are fifteen of each, so this construction is bijective. Define $\Theta(s)=d'$ by its inverse. Equivalently, the three [synthemes](../../../../../../syntheme.md) $\Theta(d)$ for $d\in s$ have common [duad](../../../../../../duad.md) $\Theta(s)$. In particular,

$$
\boxed{d\in s\quad\Longleftrightarrow\quad \Theta(s)\in\Theta(d).}
$$

For a total $T$ of $H$, map its five [synthemes](../../../../../../syntheme.md) to five [duads](../../../../../../duad.md) of $H'$. Any two of the original [synthemes](../../../../../../syntheme.md) are disjoint. Their image [duads](../../../../../../duad.md) must intersect: if two image [duads](../../../../../../duad.md) were disjoint, the unique [syntheme](../../../../../../syntheme.md) containing both in $H'$ would give a common [duad](../../../../../../duad.md) in the original two [synthemes](../../../../../../syntheme.md) through the pairs-of-totals construction. Conversely intersecting [duads](../../../../../../duad.md) cannot lie together in a [syntheme](../../../../../../syntheme.md) and give disjoint original [synthemes](../../../../../../syntheme.md). Five distinct pairwise-intersecting edges must form the full star at one point. Indeed two edges meeting at a point either force every other edge through that point or leave only the three edges of a triangle, which cannot contain five edges. Define $\Theta(T)$ to be the star's center. Distinct totals give distinct stars; since there are six of each, this is a bijection to the points of $H'$.

It remains to extend to unordered three-versus-three partitions. Start with a partition $B\mid B^c$ of $H'$. Its six cross [synthemes](../../../../../../syntheme.md) are the [perfect matchings](../../../../../../perfect-matching.md) between the two triples, parametrized by permutations in $S_3$. Two of these are disjoint exactly when the quotient of their permutations is a three-cycle. Hence the six cross [synthemes](../../../../../../syntheme.md) split into two classes of three: within a class any two are disjoint, and between classes any pair shares a [duad](../../../../../../duad.md). This unordered division into two classes is independent of the chosen orderings of the triples.

Every total has exactly two cross [synthemes](../../../../../../syntheme.md). To see this, any [syntheme](../../../../../../syntheme.md) has either one or three cross [duads](../../../../../../duad.md). If a total has $h$ all-cross [synthemes](../../../../../../syntheme.md), it covers $3h+(5-h)$ cross [duads](../../../../../../duad.md); the whole complete graph has nine, so $h=2$. Its two cross [synthemes](../../../../../../syntheme.md) belong to the same parity class. Conversely any pair in one class extends to a unique total. Thus the six totals split into two triples, the three totals arising from pairs in each parity class. Pulling them back through the original point-total bijection defines a partition $A\mid A^c$ of $H$.

Under the [duad](../../../../../../duad.md) mapping, its six internal [duads](../../../../../../duad.md) become exactly the six cross [synthemes](../../../../../../syntheme.md) of $B\mid B^c$: a [syntheme](../../../../../../syntheme.md) in a parity class belongs to the two totals formed by pairing it with the other two members. These incidences give the three edges of a triangle on each triple of totals. Therefore the partition is characterized by

$$
\boxed{d\text{ is internal to }A\mid A^c\quad\Longleftrightarrow\quad
\Theta(d)\text{ is a cross syntheme for }B\mid B^c.}
$$

This correspondence is injective: the six cross [synthemes](../../../../../../syntheme.md) determine all nine cross [duads](../../../../../../duad.md) of $K_{3,3}$, whose bipartition is unique up to interchange. There are $\binom63/2=10$ partitions on each side, so it is bijective. Define $\Theta(A\mid A^c)=B\mid B^c$ by the inverse of the construction above.

The inverse incidence rule is also useful. If a [duad](../../../../../../duad.md) $d'$ is internal to $B\mid B^c$, none of the cross [synthemes](../../../../../../syntheme.md) contains it, so its inverse [syntheme](../../../../../../syntheme.md) has no internal [duad](../../../../../../duad.md) of $A\mid A^c$ and is entirely cross. If $d'$ is cross, exactly two cross [synthemes](../../../../../../syntheme.md) contain it, so the inverse [syntheme](../../../../../../syntheme.md) has two internal [duads](../../../../../../duad.md) and one cross [duad](../../../../../../duad.md). Thus internal [duads](../../../../../../duad.md) and cross [synthemes](../../../../../../syntheme.md) exchange roles in both directions. All the extensions are natural: they use intersections and incidence, with no auxiliary ordering left in the answer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
