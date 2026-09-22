<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First the product is also split. Write $A_i=kG_i$ and $J_i=\operatorname{rad}A_i$. The ideal

$$
I=J_1\otimes A_2+A_1\otimes J_2\subset A_1\otimes A_2\cong k(G_1\times G_2)
$$

is nilpotent: if $J_1^r=J_2^s=0$, every product of $r+s-1$ of its factors vanishes. The quotient is

$$
(A_1/J_1)\otimes(A_2/J_2),
$$

a product of full [matrix algebras](../../../../../../matrix-algebra.md) over $k$, because each $A_i$ is split. A [nilpotent ideal](../../../../../../nilpotent-ideal.md) lies in the [Jacobson radical](../../../../../../jacobson-radical.md), and a semisimple quotient forces the reverse inclusion, so $I$ is exactly the radical. Thus $k$ is a [splitting field for finite group representations](../../../../../../splitting-field-for-finite-group-representations.md) of the product.

For [simple modules](../../../../../../irreducible-module.md) $S_i$, [Schur lemma](../../../../../../schur-s-lemma.md) and splitting give $\operatorname{End}_{A_i}(S_i)=k$. The [Jacobson density theorem](../../../../../../jacobson-density-theorem.md) therefore makes the image of $A_i$ on $S_i$ the full $\operatorname{End}_k(S_i)$. Tensoring these maps shows that the product algebra acts on $S_1\otimes S_2$ through its full endomorphism algebra. Hence this [tensor product of group representations](../../../../../../tensor-product-of-group-representations.md) is simple.

On restriction to $G_1$, it is a [direct sum](../../../../../../direct-sum.md) of $\dim S_2$ copies of $S_1$. If two external tensor products are isomorphic, their restrictions and the [Jordan–Hölder theorem](../../../../../../jordan-holder-theorem.md) force $S_1\cong S'_1$; restricting to $G_2$ similarly forces $S_2\cong S'_2$. The converse follows by tensoring the isomorphisms.

Finally, the p-regular conjugacy classes of $G_1\times G_2$ are precisely pairs of such classes in the factors. The corrected result in part (b) counts as many simples for the product as pairs of simples for the two factors. Our pairwise nonisomorphic tensor products already attain that count, so they exhaust all simples. Thus $\boxed{\operatorname{Irr}_k(G_1\times G_2)=\{S_1\otimes S_2\}}$, uniquely indexed by pairs of simple isomorphism classes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
