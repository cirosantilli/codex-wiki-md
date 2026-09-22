<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [class equation](../../../class-equation.md) implies that a nontrivial finite $p$-[group](../../../group-split.md) has nontrivial [center of a group](../../../center-of-a-group.md). Here a center of order $9$ would make $G/Z(G)$ cyclic; a [group](../../../group-split.md) with cyclic quotient by its [center of a group](../../../center-of-a-group.md) is abelian, contradicting the hypothesis. Thus

$$
\boxed{|Z(G)|=3,\qquad G/Z(G)\cong C_3\times C_3.}
$$

The quotient of order nine must be noncyclic for the same reason. For $x\notin Z(G)$, $\langle x,Z(G)\rangle$ has order at least nine and lies in the proper [centralizer](../../../centralizer.md) $C_G(x)$. Lagrange's theorem therefore forces $\boxed{|C_G(x)|=9}$. Also $1\ne G'\leq Z(G)$, so $G'=Z(G)$ and all [commutators](../../../commutator.md) are central of order dividing three.

**Classification and splitting.** First suppose $a$ has order nine. Then $N=\langle a\rangle$ is normal of index three and $Z(G)=\langle a^3\rangle$. For $b\notin N$, conjugation on $N$ is nontrivial, since otherwise $a,b$ would generate an abelian [group](../../../group-split.md). Its order divides three, so, after replacing $b$ by its inverse if needed, $bab^{-1}=a^4$. Write $b^3=a^{3k}$. Central [commutators](../../../commutator.md) and $3\mid\binom32$ give $(a^ib)^3=a^{3i}b^3$; choose $i=-k$ modulo three to obtain an element $c=a^ib$ of order three outside $N$. This proves

$$
\boxed{G\cong C_9\rtimes C_3,\qquad cac^{-1}=a^4.}
$$

There is a unique resulting isomorphism type, since the two nontrivial actions of order three are interchanged by reversing the complement's generator.

If there is no element of order nine, every nonidentity element has order three. Choose $a,b$ whose images form a [basis](../../../basis.md) of $G/Z(G)$ and put $c=[a,b]$. These elements generate $G$, and $c$ generates $Z(G)$. The [subgroup](../../../subgroup.md) $N=\langle a,c\rangle\cong C_3^2$ has index three and is normal. The line $\langle b\rangle$ meets $N$ trivially and complements it. Conjugation by $b$ fixes $c$ and sends $a$ to $ac$ or $ac^{-1}$; choosing the central generator removes this sign. Thus there is one isomorphism type,

$$
\boxed{G\cong C_3^2\rtimes C_3\cong\operatorname{UT}_3(\mathbb F_3),}
$$

with the nontrivial unipotent action on $\mathbb F_3^2$. These presentations are realized by the indicated [semidirect products](../../../semidirect-product.md) and have order 27. Their exponents are nine and three respectively, so they are not isomorphic. This proves both existence and completeness of the two cases.

**Their ordinary [character tables](../../../character-table.md) are the same**, up to relabelling. In either [group](../../../group-split.md) each of the 24 noncentral elements has [conjugacy class](../../../conjugacy-class.md) of size three, giving eight noncentral classes and three central singleton classes. Each noncentral class is $xZ(G)$, since conjugates of $x$ differ from $x$ by central [commutators](../../../commutator.md) and its class has size three. There are nine [linear characters](../../../linear-character.md), arising from $G/G'\cong C_3^2$, and eleven [irreducible characters](../../../irreducible-character.md) altogether. The two remaining degrees satisfy $d_1^2+d_2^2=27-9=18$, so both are three.

Put $Z(G)=\langle z\rangle$ and $\omega=e^{2\pi i/3}$. Label the noncentral classes by nonzero $(i,j)\in\mathbb F_3^2$. For $(r,s)\in\mathbb F_3^2$ the nine [linear characters](../../../linear-character.md) have values

$$
\psi_{rs}(1)=\psi_{rs}(z)=\psi_{rs}(z^2)=1,
\qquad \psi_{rs}(i,j)=\omega^{ri+sj}.
$$

At a noncentral element, [column orthogonality](../../../column-orthogonality.md) gives a squared column norm of nine. The nine [linear characters](../../../linear-character.md) already contribute nine, so both degree-three [characters](../../../character-of-a-representation.md) vanish there. By the [Schur lemma](../../../schur-s-lemma.md), a central element has value $3\omega^k$ in an irreducible representation of degree three. The central [character](../../../character-of-a-representation.md) cannot be trivial, since that would factor the representation through the abelian quotient. Orthogonality of the identity and $z$ columns then forces the two nontrivial central [characters](../../../character-of-a-representation.md) to occur once each. The final two rows, on $1,z,z^2$ and the eight other columns, are

$$
(3,3\omega,3\omega^2,0,\ldots,0),\qquad
(3,3\omega^2,3\omega,0,\ldots,0).
$$

This description gives the same entire [character table](../../../character-table.md) in both cases. The differing element orders are additional power-map data, which an ordinary [character table](../../../character-table.md) need not determine.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2011](../../2011-split.md)
3. [Past exam of the algebra course of the University of Oxford](../../split.md)
4. [Algebra course of the University of Oxford](../../../algebra-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
