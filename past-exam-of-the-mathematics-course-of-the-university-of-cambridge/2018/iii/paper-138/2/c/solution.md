<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A nonabelian [simple group](../../../../../../simple-group.md) is a [perfect group](../../../../../../perfect-group.md), so every one-dimensional [group representation](../../../../../../group-representation.md), a homomorphism to the abelian group $k^\times$, is trivial. Thus a nontrivial irreducible [Brauer character](../../../../../../brauer-character.md) cannot have degree $1$.

Suppose instead that its representation has dimension $2$, working over a splitting extension if necessary. Its determinant is a one-dimensional representation and is therefore trivial. Its kernel is a [normal subgroup](../../../../../../normal-subgroup.md), and the representation is nontrivial, so simplicity makes it faithful. Consequently $G$ embeds in $\operatorname{SL}_2(k)$.

We use the [Feit–Thompson theorem](../../../../../../feit-thompson-theorem.md): every finite group of odd order is solvable. Therefore this nonabelian simple group has even order, and [Cauchy's theorem for finite groups](../../../../../../cauchy-theorem-for-groups.md) supplies an [involution](../../../../../../involution.md) $t$. In odd [characteristic](../../../../../../characteristic-of-a-field.md), its representing matrix $A$ satisfies $A^2=I$ and is diagonalizable with [eigenvalues](../../../../../../eigenvalue.md) in $\{1,-1\}$. Since $\det A=1$, it is $I$ or $-I$. Faithfulness excludes $I$, so $t$ acts as the scalar matrix $-I$. It commutes with the whole image; faithfulness then makes $t$ central in $G$, contradicting nonabelian simplicity. Hence $\boxed{\chi(1)>2}$.

The [odd order theorem](../../../../../../feit-thompson-theorem.md) is the deep standard group-theoretic input in this proof; its use is explicit rather than hidden in an unsupported assertion that $G$ has an involution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
