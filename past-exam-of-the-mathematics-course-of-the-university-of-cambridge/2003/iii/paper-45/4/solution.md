<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\widehat T_a=\operatorname{ad}_{T_a}$ on the [Lie algebra](../../../../../lie-algebra-split.md) itself. The [Jacobi identity](../../../../../jacobi-identity.md) says, for every $X$,

$$
[T_a,[T_b,X]]-[T_b,[T_a,X]]=[[T_a,T_b],X].
$$

Therefore $[\widehat T_a,\widehat T_b]=c^c_{ab}\widehat T_c$, proving that the displayed structure-constant matrices form the [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md).

The bilinear form $\kappa_{ab}=\operatorname{tr}(\widehat T_a\widehat T_b)$ is the [Killing form](../../../../../killing-form.md). It is symmetric by cyclicity of [trace](../../../../../matrix-trace.md). Its invariance follows by expanding the two commutators:

$$
\begin{aligned}
\kappa([T_c,T_a],T_b)+\kappa(T_a,[T_c,T_b])
&=\operatorname{tr}([\widehat T_c,\widehat T_a]\widehat T_b+\widehat T_a[\widehat T_c,\widehat T_b])\\
&=\operatorname{tr}([\widehat T_c,\widehat T_a\widehat T_b])=0.
\end{aligned}
$$

In components this is precisely

$$
\boxed{\kappa_{db}c^d_{ca}+\kappa_{ad}c^d_{cb}=0.}
$$

Equivalently, the [adjoint action](../../../../../adjoint-representation-of-a-lie-group.md) preserves the bilinear form, so it is an [invariant tensor](../../../../../invariant-tensor.md).

The invariant abelian subalgebra is an abelian [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) $\mathfrak a$. Assume it is nonzero, as required for the conclusion. For $X\in\mathfrak a$ and $Y\in\mathfrak g$, the map $\operatorname{ad}_X\operatorname{ad}_Y$ sends $\mathfrak g$ into $\mathfrak a$, because it is an ideal. It vanishes on $\mathfrak a$, because $\operatorname{ad}_Y$ preserves the ideal and $\operatorname{ad}_X$ kills it. Relative to $\mathfrak a$ and a vector-space complement, this map has zero diagonal blocks, so its [trace](../../../../../matrix-trace.md) is zero. Thus

$$
\kappa(X,Y)=0\qquad(X\in\mathfrak a,\ Y\in\mathfrak g).
$$

This proves that [abelian ideals lie in the radical of the Killing form](../../../../../abelian-ideals-lie-in-the-radical-of-the-killing-form.md). Choose a nonzero $X=x^aT_a$ in the ideal. Then $\kappa_{ba}x^a=0$ for every $b$, so **the coordinate vector $x$ is a nonzero null eigenvector of the Killing matrix**. The nonzero-ideal qualification cannot be dropped: the zero ideal is abelian even in a semisimple algebra with nondegenerate [Killing form](../../../../../killing-form.md).

Now suppose $\kappa$ is invertible and let $C_\kappa=\kappa^{bc}t_bt_c$ in any [Lie algebra representation](../../../../../lie-algebra-representation.md). In matrix notation invariance is $A_a^T\kappa+\kappa A_a=0$, where $(A_a)^d{}_b=c^d_{ab}$. Multiplying by the inverse form gives $A_a\kappa^{-1}+\kappa^{-1}A_a^T=0$. Hence

$$
\begin{aligned}
[t_a,C_\kappa]
&=\kappa^{bc}(c^d_{ab}t_dt_c+c^d_{ac}t_bt_d)\\
&=(c^b_{ad}\kappa^{dc}+\kappa^{bd}c^c_{ad})t_bt_c=0.
\end{aligned}
$$

No commutativity of the representation matrices has been assumed. This proves the centrality of the [quadratic Casimir operator](../../../../../quadratic-casimir-operator.md) formed with the inverse [Killing form](../../../../../killing-form.md). [Schur lemma](../../../../../schur-s-lemma.md) makes it a scalar on every finite-dimensional complex [irreducible representation](../../../../../irreducible-representation.md).

For [SU(2)](../../../../../su-2-group.md), make the normalization explicit. In a Hermitian angular-momentum basis with $[J_a,J_b]=i\epsilon_{abc}J_c$, the structure-constant matrices obey

$$
\kappa_{ab}=\sum_{c,d}(i\epsilon_{adc})(i\epsilon_{bcd})=2\delta_{ab}.
$$

Thus $C_\kappa=\tfrac12\sum_aJ_a^2$. In the compact anti-Hermitian basis $T_a=-iJ_a$, the brackets have real structure constants $\epsilon_{abc}$ and the [Killing form of the SU(2) Lie algebra](../../../../../killing-form-of-the-su-2-lie-algebra.md) is instead $-2\delta_{ab}$; the inverse contraction gives the same $C_\kappa$. This sign change is a basis convention, not a different spectrum.

In the complex highest-weight basis $(H,E^+,E^-)$ used earlier, the same [Killing form](../../../../../killing-form.md) and its inverse are

$$
\kappa=\begin{pmatrix}8&0&0\\0&0&4\\0&4&0\end{pmatrix},\qquad \kappa^{-1}=\begin{pmatrix}1/8&0&0\\0&0&1/4\\0&1/4&0\end{pmatrix}.
$$

Consequently

$$
C_\kappa=\frac{H^2}{8}+\frac{E^+E^-+E^-E^+}{4}.
$$

On a highest vector of weight $m=2j$, the ladder calculation gives $E^+E^-v=mv$ and $E^-E^+v=0$. Its [Casimir eigenvalue](../../../../../casimir-eigenvalue.md) is therefore

$$
\boxed{\frac{m^2}{8}+\frac m4=\frac{m(m+2)}8=\frac12j(j+1),\qquad j=0,\tfrac12,1,\ldots.}
$$

Centrality gives the same value throughout the irreducible multiplet. This is the [Killing-normalized SU(2) quadratic Casimir](../../../../../killing-normalized-su-2-quadratic-casimir.md); the familiar angular-momentum operator $\sum_aJ_a^2$ has eigenvalue $j(j+1)$ and is twice this inverse-Killing-form contraction.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
