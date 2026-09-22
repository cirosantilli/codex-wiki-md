<h1 id="11e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the usual commutative, unital conventions, the chain is

$$
 \boxed{\text{field}\ \Longrightarrow\ \text{principal ideal domain}
 \ \Longrightarrow\ \text{unique factorization domain}\ \Longrightarrow\ \text{integral domain}.}
$$

A [field](../../../../../../field.md) is an [integral domain](../../../../../../integral-domain.md), and every nonzero [ideal](../../../../../../ideal.md) contains an invertible element and is consequently the whole ring. Its only [ideals](../../../../../../ideal.md) are $(0)$ and $(1)$, so it is a [principal ideal domain](../../../../../../principal-ideal-domain.md).

To prove the middle implication, first show that a [principal ideal domain](../../../../../../principal-ideal-domain.md) has the [ascending chain condition](../../../../../../ascending-chain-condition.md) on [ideals](../../../../../../ideal.md). The union of an ascending chain is an [ideal](../../../../../../ideal.md), hence is $(a)$; its generator belongs to one member of the chain, and all later members equal $(a)$. Now suppose a nonzero nonunit admitted no factorization into [irreducible elements](../../../../../../irreducible-element.md). It would factor into two nonunits, at least one of which again has no such factorization. Repeating would produce a strictly increasing chain of [principal ideals](../../../../../../principal-ideal.md): if $a=bc$ with $c$ a nonunit, $(a)\subsetneq(b)$, since equality and cancellation would make $c$ invertible. This contradicts the [ascending chain condition](../../../../../../ascending-chain-condition.md). Existence of factorization follows. By the permitted fact that every [irreducible element](../../../../../../irreducible-element.md) is a [prime element](../../../../../../prime-element.md) in a [principal ideal domain](../../../../../../principal-ideal-domain.md), any irreducible factor in one factorization divides a factor in the other; cancellation then proves uniqueness up to units and order. This is a [unique factorization domain](../../../../../../unique-factorization-domain.md). The final implication is part of the definition of a [unique factorization domain](../../../../../../unique-factorization-domain.md).

None of the adjacent implications reverses. The [principal ideal domain](../../../../../../principal-ideal-domain.md) $\mathbb Z$ is not a [field](../../../../../../field.md), since $2$ is not invertible. The [polynomial ring](../../../../../../polynomial-ring.md) $\mathbb Q[x,y]$ is a [unique factorization domain](../../../../../../unique-factorization-domain.md), by applying the polynomial extension theorem for [unique factorization domains](../../../../../../unique-factorization-domain.md) twice, but its [ideal](../../../../../../ideal.md) $(x,y)$ is not principal: a generator would divide both $x$ and $y$, so would be a unit, whereas every member of this ideal vanishes at the origin. Finally, $\mathbb Z[\sqrt{-5}]$ is an [integral domain](../../../../../../integral-domain.md) as a subring of $\mathbb C$, but is not a [unique factorization domain](../../../../../../unique-factorization-domain.md). Its multiplicative [norm](../../../../../../norm.md) is $N(a+b\sqrt{-5})=a^2+5b^2$. There is no element of norm $2$ or $3$. Hence $2,3,1+\sqrt{-5},1-\sqrt{-5}$, of norms $4,9,6,6$, are all irreducible: a nontrivial factorization would require one of those missing norms. The only units have norm one and are $\pm1$. The two factorizations

$$
 6=2\cdot3=(1+\sqrt{-5})(1-\sqrt{-5})
$$

are therefore not related by associates and reordering.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
