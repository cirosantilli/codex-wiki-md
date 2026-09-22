<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [simple group](../../../../../../simple-group.md) has no [normal subgroup](../../../../../../normal-subgroup.md) except the identity [subgroup](../../../../../../subgroup.md) and the whole group. To prove the [Simplicity of the alternating group A5](../../../../../../simplicity-of-the-alternating-group-a5.md), we compute its [conjugacy classes](../../../../../../conjugacy-class.md). Since the [sign homomorphism](../../../../../../sign-homomorphism.md) is onto, $|A_5|=5!/2=60$. Its possible nonidentity [cycle types](../../../../../../cycle-type.md) are a three-cycle, a product of two disjoint transpositions, and a five-cycle.

There are $\binom53\cdot2=20$ three-cycles. The [centralizer](../../../../../../centralizer.md) in $S_5$ of $(1\ 2\ 3)$ consists of its three powers and an independent interchange of the two unused letters. Only the three powers are even. Its [centralizer](../../../../../../centralizer.md) in $A_5$ therefore has order three, giving one [conjugacy class](../../../../../../conjugacy-class.md) of size $60/3=20$ by the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md).

There are $5\cdot3=15$ products of two disjoint transpositions: choose the fixed letter and then a pairing of the other four letters. For $(1\ 2)(3\ 4)$, a commuting [permutation](../../../../../../permutation.md) fixes $5$ and may interchange the two pairs and swap within them, giving a [centralizer](../../../../../../centralizer.md) of order eight in $S_5$. It contains an odd element, $(1\ 2)$, so exactly half its elements are even. The [centralizer](../../../../../../centralizer.md) in $A_5$ has order four, and these fifteen elements form one [conjugacy class](../../../../../../conjugacy-class.md) of size $60/4=15$.

Finally, there are $4!=24$ five-cycles. A [permutation](../../../../../../permutation.md) commuting with a five-cycle is determined by the image of one letter and must be a power of that cycle. All five powers are even, so the [centralizer](../../../../../../centralizer.md) in $A_5$ has order five. Each such [conjugacy class](../../../../../../conjugacy-class.md) has size $60/5=12$, giving two classes of size twelve.

A [normal subgroup](../../../../../../normal-subgroup.md) must be a union of [conjugacy classes](../../../../../../conjugacy-class.md) and must include the identity. Its order therefore has the form

$$
1+20a+15b+12c,\qquad a,b\in\{0,1\},\quad c\in\{0,1,2\}.
$$

The resulting distinct possibilities are

$$
1,13,16,21,25,28,33,36,40,45,48,60.
$$

Of these, only $1$ and $60$ divide $60$. [Lagrange's theorem](../../../../../../lagrange-s-theorem.md) rules out every other possible order. Hence

$$
\boxed{A_5\text{ is simple}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
