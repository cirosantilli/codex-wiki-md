<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Orient $S^3$ as the boundary of $B^4$. Push the interior of an oriented [Seifert surface](../../../../../seifert-surface.md) $F$ slightly into $B^4$, and let $X_F$ be the double [branched covering](../../../../../branched-covering.md) of $B^4$ over this pushed-in surface. Its boundary is the [two-fold branched cover of a knot](../../../../../two-fold-branched-cover-of-a-knot.md). Define the **knot signature** by

$$
\boxed{\sigma(K)=\operatorname{sign}Q_{X_F}.}
$$

The [signature](../../../../../signature-of-a-quadratic-form.md) of a possibly degenerate [intersection form](../../../../../intersection-form.md) means the number of positive eigenvalues minus the number of negative eigenvalues; its radical contributes zero.

Here is why the definition is independent of $F$. Given two choices $F_0,F_1$, glue their branched covers along the common boundary to obtain

$$
X=X_{F_0}\cup_{\Sigma_2(K)}(-X_{F_1}).
$$

This is the double [branched covering](../../../../../branched-covering.md) of $S^4$ over the closed oriented surface obtained by gluing the pushed-in $F_0$ to $-F_1$. Every closed oriented surface in $S^4$ admits a [Seifert hypersurface](../../../../../seifert-hypersurface.md): its complement has an integral meridional class, represent it by a map to the circle, and take a [regular value](../../../../../regular-value.md). Near the surface choose the angular map in its trivial normal disk bundle. The closure of a suitable regular fiber is a compact oriented three-manifold bounding the surface. Its trivial normal framing can be chosen to match this construction.

Push the interior of this [Seifert hypersurface](../../../../../seifert-hypersurface.md) into $B^5$. The double [branched covering](../../../../../branched-covering.md) of $B^5$ over the resulting properly embedded three-manifold has boundary $X$. The existence of the cover follows from the meridian homomorphism to $\mathbb Z/2$; smoothness near the branch set is the local map $(z,u)\mapsto(z^2,u)$. By the hypothesis about boundaries of five-manifolds, $\operatorname{sign}X=0$. [Novikov additivity](../../../../../novikov-additivity.md) for gluing along an entire closed three-dimensional boundary gives

$$
0=\operatorname{sign}X=\operatorname{sign}X_{F_0}-\operatorname{sign}X_{F_1}.
$$

Thus the [knot signature](../../../../../signature-of-a-knot.md) is independent of the [Seifert surface](../../../../../seifert-surface.md). An [isotopy](../../../../../isotopy.md) of the [knot](../../../../../knot.md) carries the construction to an equivalent one, so it is also a [knot invariant](../../../../../knot-invariant.md).

To calculate its [intersection form](../../../../../intersection-form.md), express $F$ as a disk with $2g$ bands. The double [branched covering](../../../../../branched-covering.md) of $B^4$ over the pushed-in disk is again $B^4$. Each band lifts to a two-handle. The capped lifted cores give a basis of $H_2(X_F;\mathbb Z)$ corresponding to the band-core basis of $H_1(F;\mathbb Z)$. The framing of the $i$th lifted attaching circle is $2\operatorname{lk}(a_i^+,a_i)=2V_{ii}$. For distinct bands, the two sheets contribute the two push-off linkings $V_{ij}$ and $V_{ji}$, so the mutual [linking number](../../../../../linking-number.md) is $V_{ij}+V_{ji}$. Hence

$$
Q_{X_F}=V+V^T,\qquad
\boxed{\sigma(K)=\operatorname{sign}(V+V^T).}
$$

A different integral basis changes this matrix by [matrix congruence](../../../../../matrix-congruence.md) and leaves its [signature](../../../../../signature-of-a-quadratic-form.md) unchanged.

In Figure 7 the upper knot is a [connected sum of knots](../../../../../connected-sum-of-knots.md) $T\mathbin{\#}T$, while the lower one is $T\mathbin{\#}\overline T$, where $T$ is the positive [trefoil knot](../../../../../trefoil-knot.md). Both [knot groups](../../../../../knot-group.md) have the **same presentation**

$$
\boxed{\langle a,b,c\mid aba=bab,\ aca=cac\rangle.}
$$

To see this, the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) expresses the [knot group](../../../../../knot-group.md) of a [connected sum of knots](../../../../../connected-sum-of-knots.md) as the [amalgamated free product](../../../../../amalgamated-free-product.md) of the two summand [knot groups](../../../../../knot-group.md), amalgamating their [meridians of a knot](../../../../../meridian-of-a-knot.md). A [trefoil knot](../../../../../trefoil-knot.md) has presentation $\langle a,b\mid aba=bab\rangle$ with $a$ a meridian. Reflection gives the same abstract group for the mirror. If it reverses the chosen meridian, send both generators to their inverses; the inverse braid relation is again the same relation. Thus the meridian amalgamation yields the displayed [group presentation](../../../../../group-presentation.md) in both cases.

A band basis for the positive [trefoil knot](../../../../../trefoil-knot.md) gives

$$
V_T=\begin{pmatrix}-1&1\\0&-1\end{pmatrix},
$$

whose symmetrization is negative definite. Therefore $\sigma(T)=-2$ and $\sigma(\overline T)=2$. Boundary-connected-summing [Seifert surfaces](../../../../../seifert-surface.md) makes the [Seifert matrix](../../../../../seifert-matrix.md) block diagonal, so the [knot signature](../../../../../signature-of-a-knot.md) is additive under [connected sum of knots](../../../../../connected-sum-of-knots.md). Consequently

$$
\boxed{\sigma(K_1)=-4,\qquad \sigma(K_2)=0.}
$$

The upper knot and lower knot are therefore not isotopic, even though their [knot groups](../../../../../knot-group.md) are isomorphic. With the opposite global [knot signature](../../../../../signature-of-a-knot.md) convention the first value is $+4$, and the distinction is unchanged.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
