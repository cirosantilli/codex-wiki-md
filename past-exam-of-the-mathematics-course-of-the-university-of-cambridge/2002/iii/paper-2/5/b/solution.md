<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Frobenius reciprocity](../../../../../../frobenius-reciprocity.md) is the adjointness of [character](../../../../../../character-of-a-representation.md) induction and restriction: for [class functions](../../../../../../class-function.md) $f$ on $H$ and $u$ on $G$,

$$
\boxed{\langle f^G,u\rangle_G=\langle f,u_H\rangle_H}.
$$

For [characters](../../../../../../character-of-a-representation.md) this says that the multiplicity of an irreducible $G$-character in an [induced character](../../../../../../induced-character.md) equals the corresponding multiplicity after restriction. To prove the identity directly, insert the induced [class function](../../../../../../class-function.md) formula and interchange the two finite sums. For each $x$, substitute $g=xhx^{-1}$ with $h\in H$. Since $u$ is constant on [conjugacy classes](../../../../../../conjugacy-class.md),

$$
\begin{aligned}
\langle f^G,u\rangle_G
&=\frac1{|G||H|}\sum_{x\in G}\sum_{h\in H}f(h)\overline{u(xhx^{-1})}\\
&=\frac1{|H|}\sum_{h\in H}f(h)\overline{u(h)}
=\langle f,u_H\rangle_H.
\end{aligned}
$$

This proves the theorem for all [class functions](../../../../../../class-function.md), not just [irreducible characters](../../../../../../irreducible-character.md).

For the group-theoretic conclusion, suppose that $p$ divides $|G'\cap Z(G)|$. A central element of order $p$ lies in every [Sylow p-subgroup](../../../../../../sylow-subgroup.md): adjoining it to a [Sylow subgroup](../../../../../../sylow-subgroup.md) gives a p-subgroup, so maximality forces it into that [subgroup](../../../../../../subgroup.md). Hence there is a [subgroup](../../../../../../subgroup.md) $Q\leq P\cap G'\cap Z(G)$ of order $p$. Choose a nontrivial [linear character](../../../../../../linear-character.md) $\lambda$ of $Q$.

Since $P$ is abelian, $\lambda$ extends to a [linear character](../../../../../../linear-character.md) $\mu$ of $P$. One direct justification is to extend from an abelian [subgroup](../../../../../../subgroup.md) $A$ to $\langle A,x\rangle$ one generator at a time: if $d$ is the least positive exponent with $x^d\in A$, choose a complex $d$th root of $\lambda(x^d)$ as the value at $x$. The formula on $ax^j$ is then well defined and multiplicative. Iteration yields the claimed extension to $P$.

The [induced character](../../../../../../induced-character.md) $\mu^G$ has degree $[G:P]$, which is prime to $p$. In its decomposition into [irreducible characters](../../../../../../irreducible-character.md), at least one constituent $\chi$ must have degree prime to $p$; otherwise the total degree would be divisible by $p$. [Frobenius reciprocity](../../../../../../frobenius-reciprocity.md) also gives $\langle\chi_P,\mu\rangle_P>0$ for this constituent. Restriction to the central [subgroup](../../../../../../subgroup.md) $Q$ forces

$$
\chi_Q=\chi(1)\lambda.
$$

Indeed, the [induced representation](../../../../../../induced-representation.md) itself restricts to $Q$ as copies of $\lambda$, because conjugation by every coset representative is trivial on $Q$; alternatively this follows from [Schur's lemma](../../../../../../schur-s-lemma.md) and the positive multiplicity after restriction.

Each $q\in Q$ consequently acts in the [representation](../../../../../../group-representation.md) affording $\chi$ as the scalar $\lambda(q)$. Taking its [determinant character](../../../../../../determinant-character.md) gives

$$
(\det\chi)_Q=\lambda^{\chi(1)}.
$$

The left side is trivial since $Q\leq G'$ and every [linear character](../../../../../../linear-character.md) kills $G'$. The right side is nontrivial since $\lambda$ has order $p$ and $p\nmid\chi(1)$. This contradiction proves

$$
\boxed{p\nmid|G'\cap Z(G)|}.
$$

The argument is the [central commutator has no torsion from an abelian Sylow subgroup](../../../../../../central-commutator-has-no-torsion-from-an-abelian-sylow-subgroup.md) determinant obstruction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
