<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [monoidal category](../../../../../monoidal-category.md) consists of a [category](../../../../../category-split.md) $\mathcal C$, a bifunctor $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a [monoidal unit object](../../../../../monoidal-unit-object.md) $I$, and natural isomorphisms

$$
\alpha_{A,B,C}:(A\otimes B)\otimes C\longrightarrow A\otimes(B\otimes C),\qquad\lambda_A:I\otimes A\longrightarrow A,\qquad\rho_A:A\otimes I\longrightarrow A.
$$

The [associator](../../../../../associator.md) and [unitors](../../../../../unitor.md) satisfy the [pentagon identity for a monoidal category](../../../../../pentagon-identity-for-a-monoidal-category.md)

$$
\alpha_{A,B,C\otimes D}\,\alpha_{A\otimes B,C,D}=(1_A\otimes\alpha_{B,C,D})\,\alpha_{A,B\otimes C,D}\,(\alpha_{A,B,C}\otimes1_D),
$$

and the [triangle identity for a monoidal category](../../../../../triangle-identity-for-a-monoidal-category.md)

$$
(1_A\otimes\lambda_B)\,\alpha_{A,I,B}=\rho_A\otimes1_B.
$$

Composition is written from right to left. Naturality of these isomorphisms is part of the definition.

A [symmetric monoidal category](../../../../../symmetric-monoidal-category.md) additionally has a natural [braiding](../../../../../braiding.md) $c_{A,B}:A\otimes B\to B\otimes A$ with $c_{B,A}c_{A,B}=1$, satisfying the two hexagon identities. Written as composites from the same source to the same target, these are

$$
\begin{aligned}
c_{A,B\otimes C}&=\alpha_{B,C,A}^{-1}(1_B\otimes c_{A,C})\alpha_{B,A,C}(c_{A,B}\otimes1_C)\alpha_{A,B,C}^{-1},\\
c_{A\otimes B,C}&=\alpha_{C,A,B}(c_{A,C}\otimes1_B)\alpha_{A,C,B}^{-1}(1_A\otimes c_{B,C})\alpha_{A,B,C}.
\end{aligned}
$$

The unit compatibility is $c_{A,I}=\lambda_A^{-1}\rho_A$ and $c_{I,A}=\rho_A^{-1}\lambda_A$.

For two distinct choices of symmetry, take [super vector spaces](../../../../../super-vector-space.md) over $\mathbb Q$, with degree-preserving linear maps, the usual graded [tensor product](../../../../../tensor-product.md), its usual associator, and the unit concentrated in degree zero. On vectors of degrees $p,q\in\{0,1\}$, define

$$
c^{(0)}(v\otimes w)=w\otimes v,\qquad c^{(1)}(v\otimes w)=(-1)^{pq}w\otimes v.
$$

Both are natural in degree-preserving maps and are involutive. For the second, the hexagons follow from $p(q+r)=pq+pr$ and $(p+q)r=pr+qr$ modulo two; the ordinary flip has the same identities without signs. Degree zero of the unit gives unit compatibility. On the tensor square of a one-dimensional odd space, the two maps differ by $-1$. Thus **the same monoidal structure can carry two different symmetries**; the second uses the [Koszul sign rule](../../../../../koszul-sign-rule.md).

We prove the [monoidal coherence theorem](../../../../../monoidal-coherence-theorem.md) by a terminating normalization argument. Its precise formal assertion is that any two composites of associators, unitors, their inverses, and their tensor products with identities, between the same formal tensor expressions, are equal. The expressions must have the same ordered list of object letters after unit symbols are removed. This does not assert that different symmetries are equal, nor does it treat an accidental equality of actual objects as a new structural identification.

Use the following directed reductions in every tensor context:

$$
((A\otimes B)\otimes C)\longrightarrow A\otimes(B\otimes C),\qquad I\otimes A\longrightarrow A,\qquad A\otimes I\longrightarrow A,
$$

interpreted respectively by $\alpha$, $\lambda$, $\rho$. For a formal expression $T$, let $\ell(T)$ be its number of leaves, counting both object letters and unit symbols, and define

$$
w(A)=w(I)=0,\qquad w(S\otimes T)=w(S)+w(T)+\ell(S).
$$

Order the pairs $(\ell,w)$ by comparing the first coordinate first, and then the second. A unit reduction decreases the first coordinate. An associativity reduction preserves the first coordinate and decreases the second by $\ell(A)>0$. The same calculation holds in any context, since associativity preserves the size of the rewritten subtree. Hence there is no infinite directed reduction path.

An irreducible expression has no unit next to another tensor factor and no composite left tensor factor. It is therefore the right-associated expression of its ordered nonunit letters, or the single unit $I$ if there are no such letters. In particular the normal form is uniquely determined by the ordered word.

We next show that every pair of first reductions has a commuting completion. Reductions in disjoint subexpressions commute by bifunctoriality of the [monoidal tensor product](../../../../../monoidal-tensor-product.md). A reduction inside one of the variable expressions $A,B,C$ commutes with the outer reduction by [naturality](../../../../../naturality.md) of the associator or unitor. The genuine overlaps are exactly the following cases.

For $(((A\otimes B)\otimes C)\otimes D)$, associating first at the root or first in its left subtree gives the two sides of the pentagon; their completions to $A\otimes(B\otimes(C\otimes D))$ commute.

For $((I\otimes A)\otimes B)$, the competing associator and inner left unitor have a commuting completion because

$$
\lambda_{A\otimes B}\,\alpha_{I,A,B}=\lambda_A\otimes1_B.
$$

For $((A\otimes I)\otimes B)$, the analogous completion is exactly the triangle identity. For $((A\otimes B)\otimes I)$, the associator and the outer right unitor have a commuting completion because

$$
\rho_{A\otimes B}=(1_A\otimes\rho_B)\,\alpha_{A,B,I}.
$$

The two displayed unit identities are the permitted [unit identities derived from the monoidal pentagon and triangle](../../../../../unit-identities-derived-from-the-monoidal-pentagon-and-triangle.md).

The final overlap is $I\otimes I$, where both unitors apply. They agree as a consequence of the same identities. Naturality of $\lambda$ at the map $\lambda_I:I\otimes I\to I$, followed by cancellation of $\lambda_I$, gives

$$
\lambda_{I\otimes I}=1_I\otimes\lambda_I.
$$

Therefore left-unit compatibility and the triangle give

$$
\lambda_I\otimes1_I=\lambda_{I\otimes I}\alpha_{I,I,I}=(1_I\otimes\lambda_I)\alpha_{I,I,I}=\rho_I\otimes1_I.
$$

The [functor](../../../../../functor.md) $-\otimes I$ is naturally isomorphic to the identity via $\rho$, and is consequently faithful. Thus $\lambda_I=\rho_I$, so this overlap commutes too. There are no other nonvariable overlaps among the three reduction patterns.

Termination and these commuting completions imply equality of all normalization arrows, not merely uniqueness of the normal-form object. Here is the induction. Suppose every expression smaller than $T$ in the decreasing pair measure has a unique normalization arrow. Two normalization paths from $T$ start with arrows $r:T\to T_1$ and $s:T\to T_2$. The local completion gives directed paths $d_1:T_1\to V$, $d_2:T_2\to V$ with $d_1r=d_2s$. Append any normalization $\nu_V$ of $V$. By the induction hypothesis the tails of the original paths are $\nu_Vd_1$ and $\nu_Vd_2$. Their composites from $T$ are equal. If $T$ is already normal, its only directed normalization is the identity. This proves the induction.

Write $\nu_T:T\to N(T)$ for the resulting unique normalization. For every directed structural generator $g:S\to T$, including a generator in an arbitrary tensor context, uniqueness gives $\nu_Tg=\nu_S$. Since all structural generators are invertible, the corresponding equation holds for their inverses as well. Any structural composite $f:S\to T$ consequently satisfies

$$
\boxed{f=\nu_T^{-1}\nu_S.}
$$

Its value depends only on the formal endpoints. Thus every structural diagram with the specified ordered word commutes, proving the [monoidal coherence theorem](../../../../../monoidal-coherence-theorem.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
