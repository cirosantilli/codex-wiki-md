<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a faithful transitive ordered action, primitivity here means that the only invariant equivalence relations with convex classes are equality and the universal relation. The trichotomy is: a regular Archimedean action, an order two-transitive action, or a periodic action. In the regular case the chain is an ordered additive subgroup of $\mathbb R$, acting by translations. In the periodic case there is a fixed-point-free period $z$ on the [Dedekind completion](../../../../../../dedekind-completion.md), commuting with the action and having cofinal and coinitial integer iterates; inside a period interval the relevant stabilizer acts order two-transitively. These are the cases of the [McCleary trichotomy theorem](../../../../../../mccleary-trichotomy-theorem.md).

**Only the regular Archimedean case satisfies the inequality.** It is a [linearly ordered group](../../../../../../linearly-ordered-group.md). For positive $a,b$, if $a\le b$, then $ab\le b^2\le b^2a^2$; if $b\le a$, then $ab\le a^2\le b^2a^2$. Taking $a=|f|$, $b=|g|$ proves the displayed inequality.

To exclude an order two-transitive action, choose $x<y<z<t$. Choose an automorphism taking $(x,y)$ to $(y,z)$ and replace it by its pointwise [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) with the identity, giving positive $a$ with $xa=y$, $ya=z$. Similarly obtain positive $b$ with $xb=x$, $yb=t$. Then

$$
xab=t>z=xb^2a^2.
$$

Thus $ab\not\le b^2a^2$, while $|a|=a$ and $|b|=b$. The same construction inside a period interval excludes the periodic case, using the order two-transitive stabilizer supplied by the classification.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
