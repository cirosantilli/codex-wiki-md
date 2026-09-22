<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [M-group](../../../../../monomial-group.md) is a finite group for which every [irreducible character](../../../../../irreducible-character.md) is induced from a [linear character](../../../../../linear-character.md) of some subgroup. Let $L\triangleleft K$ have both $L$ and $K/L$ abelian, and fix an irreducible $K$-module $V$ with character $\chi$. Since $L$ is abelian, $V_L$ has a linear constituent. Choose, among all pairs $(A,\varphi)$ with $L\subseteq A\subseteq K$ and a [linear character](../../../../../linear-character.md) $\varphi$ occurring in $\chi_A$, one for which $|A|$ is maximal.

Every subgroup containing $L$ is normal in $K$: its image in the abelian quotient $K/L$ is normal, and it is the full preimage of that image. Thus $A\triangleleft K$, so the [inertia group of a character](../../../../../inertia-group-of-a-character.md) $I_K(\varphi)$ is defined and contains $A$.

Suppose $x\in I_K(\varphi)\setminus A$. The nonzero $\varphi$-[isotypic component](../../../../../isotypic-component.md) $V_\varphi$ is preserved by $x$, and every $a\in A$ acts there as the scalar $\varphi(a)$ because $\varphi(1)=1$. The finite-order operator representing $x$ is diagonalizable over $\mathbb C$; choose an eigenvector $0\ne v\in V_\varphi$. Then $\mathbb Cv$ is invariant under both $A$ and $x$, hence under $D=\langle A,x\rangle$. This line affords a [linear character](../../../../../linear-character.md) $\psi$ of $D$ with $\psi_A=\varphi$. Since it is a subrepresentation of $V_D$, it is a constituent of $\chi_D$. But $D$ strictly contains $A$ and still contains $L$, contradicting maximality.

Therefore $I_K(\varphi)=A$. Apply the [Clifford correspondence](../../../../../clifford-correspondence.md) with [normal subgroup](../../../../../normal-subgroup.md) $A$. Its inertia group is $A$ itself, and $\operatorname{Irr}(A\mid\varphi)=\{\varphi\}$, so the unique irreducible $K$-character lying over $\varphi$ is $\varphi^K$. In particular,

$$
\boxed{\chi=\varphi^K,\qquad\varphi(1)=1.}
$$

Since $\chi$ was arbitrary, every [irreducible character](../../../../../irreducible-character.md) is a [monomial character](../../../../../monomial-character.md), proving that [finite metabelian groups are monomial](../../../../../finite-metabelian-groups-are-monomial.md):

$$
\boxed{\text{Every finite metabelian group is an M-group}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
