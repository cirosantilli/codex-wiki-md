<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Wirtinger presentation](../../../../../wirtinger-presentation.md) assigns a meridian generator to each arc between undercrossings. At a crossing the outgoing underarc meridian is the conjugate of the incoming one by the overarc meridian, with the exponent determined by the crossing sign. One crossing relation is redundant for a connected [knot](../../../../../knot.md) diagram. This gives a presentation of the [knot group](../../../../../knot-group.md), the [fundamental group](../../../../../fundamental-group.md) of its exterior.

For the [trefoil knot](../../../../../trefoil-knot.md), choose three arcs x,y,z so that two crossing relations are $z=xyx^{-1}$ and $x=yzy^{-1}$. The third follows from these. Substituting for z gives $xyx=yxy$, hence

$$
\boxed{\pi_1(S^3\setminus T)=\langle x,y\mid xyx=yxy\rangle.}
$$

We use the relator $r=xyxy^{-1}x^{-1}y^{-1}$.

Here is the [Fox free differential calculus](../../../../../fox-calculus.md), including its connection with the covering-space chain complex. Let F be the [free group](../../../../../free-group.md) on $x_1,\ldots,x_n$, let $\mathbb ZF$ be its [group ring](../../../../../group-ring.md), and let $\varepsilon:\mathbb ZF\to\mathbb Z$ be augmentation. Define additive maps $D_j:\mathbb ZF\to\mathbb ZF$ by

$$
D_j(x_i)=\delta_{ij},\qquad D_j(ab)=D_j(a)\varepsilon(b)+aD_j(b),\qquad D_j(1)=0.
$$

For [group](../../../../../group-split.md) words u,v the product rule reads $D_j(uv)=D_j(u)+uD_j(v)$. Differentiating $x_ix_i^{-1}=1$ forces $D_j(x_i^{-1})=-\delta_{ij}x_i^{-1}$. Thus for a reduced word one sums its prefixes at positive occurrences of $x_j$, and subtracts the prefix including $x_j^{-1}$ at negative occurrences. Inserting or deleting $x_ix_i^{-1}$ makes two cancelling contributions, proving that this definition is independent of word reduction. Linear extension proves the group-ring product rule and uniqueness.

The fundamental identity is

$$
w-1=\sum_{j=1}^nD_j(w)(x_j-1).
$$

It holds on generators and inverses. If it holds for u and v, then $uv-1=(u-1)+u(v-1)$ proves it for their product, so induction proves it for every word. These [Fox derivatives](../../../../../fox-derivative.md) form the [matrix](../../../../../matrix.md) $\big(D_jr_i\big)_{i,j}$ for any chosen presentation.

Let $\phi:G\to\mathbb Z$ be knot-group [abelianization](../../../../../abelianization.md) and put $a_j=\phi(x_j)$. Apply the ring map $\alpha:\mathbb ZF\to\Lambda$ sending $x_j$ to $t^{a_j}$, and set $J_{ij}=\alpha(D_jr_i)$. Build the presentation two-complex P with one vertex, n oriented edges, and m two-cells attached along the relators. Its [infinite cyclic cover](../../../../../infinite-cyclic-cover-of-a-knot-exterior.md) has [cellular chain complex](../../../../../cellular-chain-complex.md)

$$
\Lambda^m\xrightarrow{\,J^T\,}\Lambda^n\xrightarrow{\,d_1\,}\Lambda,\qquad d_1(e_j)=t^{a_j}-1.
$$

To verify the second boundary, lift an attaching word starting at deck level zero. An occurrence $x_j$ after prefix u traverses the jth edge at level $\phi(u)$, contributing $t^{\phi(u)}e_j$. An occurrence $x_j^{-1}$ traverses it backwards starting at level $\phi(ux_j^{-1})$, contributing $-t^{\phi(ux_j^{-1})}e_j$. Their sum is exactly the evaluated Fox derivative. The fundamental identity, with $\alpha(r_i)=1$, gives $d_1J^T=0$.

The cover of P and the cover of the [knot exterior](../../../../../knot-exterior.md) both have [fundamental group](../../../../../fundamental-group.md) $\ker\phi$. Their first [homology](../../../../../homology-split.md) is the [abelianization](../../../../../abelianization.md) of that [group](../../../../../group-split.md), with the same deck action induced by conjugation. Thus no assumption that the presentation complex is aspherical is needed, and the complete relation with the [Alexander module of a knot](../../../../../alexander-module-of-a-knot.md) is

$$
\boxed{\mathcal A_K\cong\ker d_1/\operatorname{im}J^T.}
$$

For meridian generators all $a_j=1$. Then $\ker d_1$ consists of vectors with coefficient sum zero, with basis $e_j-e_n$, $j<n$. Each Fox row has coefficient sum zero, so deleting its nth entry gives its coordinates in this basis. Deleting one column of J therefore presents the [Alexander module](../../../../../alexander-module-of-a-knot.md); if a Wirtinger relator is redundant it can also be deleted. This proves the [matrix](../../../../../matrix.md) procedure used for the displayed [knot](../../../../../knot.md) above. For arbitrary generators, the exponent vector is primitive because the generators map onto $\mathbb Z$; elementary changes of free generators implement the Euclidean algorithm and reduce it to $(1,0,\ldots,0)$. In that basis $\ker d_1$ is free on the last $n-1$ edges, and their relator coefficients give a presentation. This explains the general case rather than treating the full Fox cokernel as the [Alexander module](../../../../../alexander-module-of-a-knot.md).

For the trefoil relator, with $\alpha(x)=\alpha(y)=t$, direct differentiation gives

$$
\alpha(D_xr)=1-t+t^2=f(t),\qquad\alpha(D_yr)=t-t^2-1=-f(t).
$$

The first boundary is $(t-1,t-1)$, whose kernel is generated by $(1,-1)$. The relator boundary is $f(t)(1,-1)$, whence

$$
\boxed{\mathcal A_T\cong\Lambda/(t^2-t+1),\qquad\Delta_T(t)\doteq t^2-t+1.}
$$

For a [connected sum of knots](../../../../../connected-sum-of-knots.md), join [Seifert surfaces](../../../../../seifert-surface.md) in separated balls. Their [Seifert matrix](../../../../../seifert-matrix.md) is block diagonal, so the [Alexander module of a connected sum](../../../../../alexander-module-of-a-connected-sum.md) is a direct sum. Thus $\mathcal A_{T\#T}\cong(\Lambda/(f))^2$.

This [module](../../../../../module-mathematics.md) is not cyclic. The [polynomial](../../../../../polynomial-split.md) f is irreducible modulo two, since it has no root in $\mathbb F_2$, so $\mathfrak m=(2,f)$ is a [maximal ideal](../../../../../maximal-ideal.md) of $\Lambda$ with [residue field](../../../../../residue-field.md) $\mathbb F_4$. The quotient $\mathcal A_{T\#T}/\mathfrak m\mathcal A_{T\#T}$ has dimension two over that field, whereas the corresponding quotient of a [cyclic module](../../../../../cyclic-module.md) has dimension at most one.

Every two-generator [knot group](../../../../../knot-group.md), however, has a cyclic [Alexander module](../../../../../alexander-module-of-a-knot.md), regardless of its number of relators. Indeed its primitive [abelianization](../../../../../abelianization.md) vector can be changed to $(1,0)$ as above. The covering boundary is then $(t-1,0)$; its kernel is the free rank-one [module](../../../../../module-mathematics.md) on the second edge, and any quotient by lifted relators is cyclic. This proves the [two-generator knot groups have cyclic Alexander modules](../../../../../two-generator-knot-groups-have-cyclic-alexander-modules.md) obstruction. Consequently **the [group](../../../../../group-split.md) of the connected sum of two trefoils cannot even be generated by two elements**, and in particular it has no two-generator, one-relator presentation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
