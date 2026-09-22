<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Assume first $n\ge2$. All [transpositions](../../../../../../../transposition-permutation.md) form a single [conjugacy class](../../../../../../../conjugacy-class.md) $T_1$. A [group automorphism](../../../../../../../group-automorphism.md) preserves [order of a group element](../../../../../../../order-of-a-group-element.md), so the image of a [transposition](../../../../../../../transposition-permutation.md) is a nonidentity [involution](../../../../../../../involution.md). By the order formula, its [disjoint cycle decomposition](../../../../../../../disjoint-cycle-decomposition.md) contains only one-cycles and two-cycles, with at least one two-cycle. Thus it lies in some $T_k$, where $1\le k\le\lfloor n/2\rfloor$.

Moreover an [automorphism](../../../../../../../automorphism.md) maps the entire [conjugacy class](../../../../../../../conjugacy-class.md) onto the [conjugacy class](../../../../../../../conjugacy-class.md) of the image: for a fixed [transposition](../../../../../../../transposition-permutation.md) $t$,

$$
\phi(gtg^{-1})=\phi(g)\phi(t)\phi(g)^{-1},
$$

and $\phi(g)$ runs over all of $S_n$ by surjectivity. Part (a)(i) identifies that latter [conjugacy class](../../../../../../../conjugacy-class.md) as $T_k$. Hence $\boxed{\phi(T_1)=T_k}$, with equality rather than just inclusion. If $n=1$, $T_1$ is empty and the equality holds trivially with $k=1$.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
