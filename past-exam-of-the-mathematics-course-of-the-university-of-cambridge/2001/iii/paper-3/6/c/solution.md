<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $n=6$ in part (b). The quotient $W=u^\perp/\langle u\rangle$ has dimension four and a [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) alternating form. The coordinate action therefore defines

$$
\rho:S_6\longrightarrow Sp(W)\cong Sp(4,2).
$$

Prove it is faithful before comparing orders. If a [permutation](../../../../../../permutation.md) lies in the [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md), it fixes the quotient class of each two-element subset $A$. That class has exactly the two representatives $A$ and $A+\Omega=\Omega\setminus A$. Their cardinalities are two and four. A coordinate [permutation](../../../../../../permutation.md) preserves cardinality, so it must fix $A$ itself, not exchange it with its complement. Thus it fixes every two-element subset. Intersecting the fixed sets $\{i,j\}$ and $\{i,k\}$ shows it fixes each singleton $\{i\}$, so it is the identity. Hence $\rho$ is injective.

By part (a),

$$
|Sp(4,2)|=2^4(2^2-1)(2^4-1)=16\cdot3\cdot15=720=6!.
$$

An injection between [finite groups](../../../../../../finite-group.md) of equal order is surjective. Choosing a [symplectic basis](../../../../../../symplectic-basis.md) of $W$ identifies the form with the standard one, so

$$
\boxed{Sp(4,2)\cong S_6.}
$$

This realizes the exceptional isomorphism through a concrete binary [permutation](../../../../../../permutation.md) module. Equality of orders alone would not establish it; the faithful form-preserving action supplies the required [group homomorphism](../../../../../../group-homomorphism.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
