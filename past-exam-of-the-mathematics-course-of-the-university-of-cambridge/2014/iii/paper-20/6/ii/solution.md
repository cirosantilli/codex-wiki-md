<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $\mathcal A$ to be the category of finitely presented [commutative rings](../../../../../../commutative-ring.md) with identity, and put $\mathcal C=\mathcal A^{\mathrm{op}}$. In its presheaf topos, the tautological ring $U(A)=A$ is generic. The additional domain axioms are [coherent sequents](../../../../../../coherent-sequent.md), so they are imposed by a [quotient-theory coverage](../../../../../../quotient-theory-coverage.md) on $\mathcal C$.

Concretely, declare the zero ring covered by the empty family. For every finitely presented $A$ and elements $a,b\in A$ with $ab=0$, declare the two opposite quotient arrows associated with

$$
\boxed{A\longrightarrow A/(a),\qquad A\longrightarrow A/(b)}
$$

to be a covering family at $A$. These [quotient rings](../../../../../../quotient-ring.md) are finitely presented. [Pullback](../../../../../../pullback-category-theory.md) and transitivity generate a Grothendieck topology $J$ from these families. The empty cover forbids $0=1$; the two quotient covers make every zero product locally have a zero factor. Conversely, any internal integral domain satisfies exactly the continuity conditions prescribed by these generating covers. Thus

$$
\boxed{\mathbf{Sh}(\mathcal A^{\mathrm{op}},J)\text{ classifies integral domains},}
$$

and its generic domain is the associated sheaf $K=a_JU$, with the ring operations transported through the left-exact sheaf reflector.

This coverage is **not standard**, meaning not all [representables](../../../../../../representable-functor.md) are sheaves; in modern terminology it is not subcanonical. For an explicit obstruction, use $A=\mathbb Z/4\mathbb Z$ and $a=b=2$. The two quotient arrows are the same map $A\to\mathbb Z/2\mathbb Z$, so their generated sieve is a singleton cover. Consider the [representable](../../../../../../representable-functor.md) on $\mathcal C$ corresponding to $R=\mathbb Z[t]$:

$$
yR(A)=\operatorname{Hom}_{\mathrm{Ring}}(R,A).
$$

Its distinct sections $t\mapsto0$ and $t\mapsto2$ become equal after restriction to $\mathbb Z/2\mathbb Z$. Hence this [representable](../../../../../../representable-functor.md) is not even separated for $J$. The [nilpotent element](../../../../../../nilpotent.md) has to disappear in the generic domain, which explains this failure of standardness.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Section B](../../section-b.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
