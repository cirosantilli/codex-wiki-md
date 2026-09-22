<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the degree-one convention implicit in this enveloping-algebra assertion: a [degree-one almost commutative algebra](../../../../../../degree-one-almost-commutative-algebra.md) has $F_0R=k$, a finite-dimensional $F_1R$ containing $1$ which generates $R$, and commutative [associated graded ring](../../../../../../associated-graded-ring.md). Taking the leading symbol of a [commutator](../../../../../../commutator.md) gives

$$
[F_iR,F_jR]\subseteq F_{i+j-1}R,
$$

in particular $[F_1R,F_1R]\subseteq F_1R$. Thus $\mathfrak g=F_1R$, equipped with $[u,v]=uv-vu$, is a finite-dimensional [Lie algebra](../../../../../../lie-algebra-split.md). Bilinearity and antisymmetry are immediate, and expanding the three nested [commutators](../../../../../../commutator.md) proves the [Jacobi identity](../../../../../../jacobi-identity.md).

Its inclusion into the associative [algebra](../../../../../../algebra-split.md) $R$ is a [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md). The [universal enveloping algebra](../../../../../../universal-enveloping-algebra.md) is $T(\mathfrak g)$ modulo the relations $u\otimes v-v\otimes u-[u,v]$. Sending the tensor generators to their elements of $R$ kills these relations and gives an [algebra homomorphism](../../../../../../algebra-homomorphism-over-a-field.md) $U(\mathfrak g)\to R$. It is surjective because $F_1R$ generates $R$. Therefore

$$
\boxed{R\cong U(\mathfrak g)/\ker(U(\mathfrak g)\to R),\qquad \dim_k\mathfrak g<\infty.}
$$

The vector $1\in F_1R$ is retained as a central [Lie algebra](../../../../../../lie-algebra-split.md) generator and maps to the associative identity; its corresponding relation in the kernel is that generator minus $1_{U(\mathfrak g)}$. One should not first replace $F_1R$ by $F_1R/k1$, since [commutators](../../../../../../commutator.md) of generators can be nonzero scalars.

Terminology is important here. Merely requiring a commutative finitely generated [associated graded ring](../../../../../../associated-graded-ring.md) for an arbitrary weighted [filtration](../../../../../../filtration-probability-theory.md) is a broader definition of [almost commutative algebra](../../../../../../almost-commutative-algebra.md); it does not supply the finite-dimensional bracket-closed first step used in this argument. The degree-one assumptions make the requested enveloping presentation precise. The Noetherianity in part (b) also follows directly under the broader finite-generation convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
