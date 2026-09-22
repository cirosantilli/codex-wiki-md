<h1 id="1b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $y=gxg^{-1}$, cancellation of successive $g^{-1}g$ factors gives $y^k=gx^kg^{-1}$ for every positive integer $k$. Hence $y^k$ is the [identity element](../../../../../../identity-element.md) exactly when $x^k$ is, proving that [conjugate group elements](../../../../../../conjugate-group-elements.md) have the same [order of a group element](../../../../../../order-of-a-group-element.md). For [permutations](../../../../../../permutation.md), the sign [group homomorphism](../../../../../../group-homomorphism.md) similarly gives

$$
\operatorname{sgn}(gxg^{-1})=\operatorname{sgn}(g)\operatorname{sgn}(x)\operatorname{sgn}(g)^{-1}=\operatorname{sgn}(x).
$$

Thus [conjugate permutations](../../../../../../conjugate-permutation.md) have the same [sign of a permutation](../../../../../../sign-of-a-permutation.md).

The converse is false: [permutation order and sign do not determine conjugacy](../../../../../../permutation-order-and-sign-do-not-determine-conjugacy.md). In the [symmetric group](../../../../../../symmetric-group.md) $S_6$, take $x=(123)$ and $y=(123)(456)$. Both have order three and positive sign. However, $x$ fixes three symbols whereas $y$ fixes none. If $x$ fixes a symbol $j$, then $gxg^{-1}$ fixes $g(j)$, and applying the inverse conjugation gives a bijection between the fixed-symbol sets. Their different fixed-point counts therefore prove that $x,y$ are not conjugate. Equivalently their [cycle types](../../../../../../cycle-type.md) $3\,1^3$ and $3^2$ differ. **Equal order and sign are necessary, but not sufficient, for conjugacy.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1B](../../1b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
