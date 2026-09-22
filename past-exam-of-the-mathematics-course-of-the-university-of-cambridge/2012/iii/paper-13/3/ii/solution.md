<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $x,y$ for the two coordinates. The PDF gives $\mu=e^{\pi i/3}$, a primitive sixth root of unity. The matrices satisfy

$$
\sigma^6=1,\qquad \tau^2=-I=\sigma^3,\qquad
\tau\sigma\tau^{-1}=\sigma^{-1}.
$$

These relations reduce every word to $\sigma^j$ or $\tau\sigma^j$, $0\le j<6$. The six first matrices are diagonal and distinct, and the six second matrices are antidiagonal and distinct. Thus **$G$ has exactly twelve elements**; it is a [binary dihedral group](../../../../../../dicyclic-group.md).

First calculate the [polynomial invariant ring](../../../../../../polynomial-invariant-ring.md) of $\langle\sigma\rangle$. A monomial $x^a y^b$ is invariant exactly when $a-b$ is divisible by $6$. Removing the smaller exponent shows that it is a product of powers of

$$
A=x^6,\qquad B=y^6,\qquad C=xy.
$$

The sole relation is $AB=C^6$. Indeed, reduction by this relation leaves monomials $C^jA^a$ and $C^jB^b$ with $b>0$, whose images in $\mathbb C[x,y]$ have distinct exponent pairs. Hence

$$
\mathbb C[x,y]^{\langle\sigma\rangle}
\cong\mathbb C[A,B,C]/(AB-C^6).
$$

On these generators, $\tau$ interchanges $A,B$ and sends $C$ to $-C$. Put $S=A+B$ and $T=A-B$. Since $2$ is invertible, the preceding [ring](../../../../../../ring.md) is

$$
\mathbb C[S,C,T]/(T^2-S^2+4C^6).
$$

Every element has a unique form $P(S,C)+TQ(S,C)$. The induced involution fixes $S$ and negates both $C$ and $T$. Its invariants are therefore exactly the expressions

$$
P_0(S,C^2)+CTQ_0(S,C^2).
$$

Set

$$
U=x^6+y^6,\qquad V=x^2y^2,\qquad W=xy(x^6-y^6).
$$

We obtain the relation

$$
W^2=V(U^2-4V^3).
$$

The unique normal form above also proves that there are no further relations: $P_0(U,V)+WQ_0(U,V)=0$ forces both polynomials to vanish. Thus the [polynomial invariant ring](../../../../../../polynomial-invariant-ring.md) is

$$
\boxed{\mathbb C[x,y]^G\cong
\mathbb C[U,V,W]/(W^2-VU^2+4V^4).}
$$

For completeness, the [algebraic quotient by a finite group](../../../../../../algebraic-quotient-by-a-finite-group.md) is the [affine variety](../../../../../../affine-algebraic-set.md) with this [coordinate ring](../../../../../../coordinate-ring.md). Each element $h$ of $\mathbb C[x,y]$ satisfies the monic orbit polynomial $\prod_{g\in G}(Z-g h)$ with invariant coefficients, so the quotient map is a [finite morphism](../../../../../../finite-morphism.md). Invariants separate distinct finite orbits: interpolate a [polynomial](../../../../../../polynomial-split.md) taking value $0$ on one orbit and $1$ on the other, and average it over $G$. Thus its fibres are precisely the orbits. The defining polynomial and resulting [algebraic quotient by a finite group](../../../../../../algebraic-quotient-by-a-finite-group.md) are

$$
\boxed{p(U,V,W)=W^2-VU^2+4V^4,\qquad
\mathbb A^2/G\cong V(p)\subset\mathbb A^3.}
$$

Using the converted TeX's fourth root would instead give a different group and a different [binary dihedral invariant hypersurface](../../../../../../binary-dihedral-invariant-hypersurface.md); the sixth root from the original PDF is essential.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
