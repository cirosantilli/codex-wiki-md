<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let F be an oriented genus-g [Seifert surface](../../../../../seifert-surface.md) for K, and choose a basis $a_1,\ldots,a_{2g}$ of $H_1(F;\mathbb Z)$. Push a representative curve slightly in the positive normal direction to obtain $a_i^+$. The [Seifert matrix](../../../../../seifert-matrix.md) in our row convention is

$$
V_{ij}=\operatorname{lk}(a_i^+,a_j).
$$

The difference $V-V^T$ is the [intersection form](../../../../../intersection-form.md) of F, up to the convention for its [orientation](../../../../../orientation-of-a-simplex.md); in a symplectic basis it is a direct sum of unimodular two-by-two skew blocks.

Write $X=S^3\setminus\operatorname{int}N(K)$ for the [knot exterior](../../../../../knot-exterior.md). Linking number with K gives the epimorphism $\pi_1(X)\to\mathbb Z$ sending a positive meridian to one. Let $\widetilde X$ be the associated [infinite cyclic cover](../../../../../infinite-cyclic-cover-of-a-knot-exterior.md), with [deck transformation](../../../../../deck-transformation.md) t. The [Alexander module of a knot](../../../../../alexander-module-of-a-knot.md) is $\mathcal A_K=H_1(\widetilde X;\mathbb Z)$, regarded as a [module](../../../../../module-mathematics.md) over the [Laurent polynomial ring](../../../../../laurent-polynomial-ring.md) $\Lambda=\mathbb Z[t,t^{-1}]$. Its order, the greatest common divisor of the maximal presentation minors, is the [Alexander polynomial of a knot](../../../../../alexander-polynomial.md), defined up to $\pm t^k$. Equivalently these minors generate its zeroth [Fitting ideal](../../../../../fitting-ideal.md); we will obtain a square presentation, so its [determinant](../../../../../determinant.md) gives the order. No assertion that $\Lambda$ is a [principal ideal domain](../../../../../principal-ideal-domain.md) is needed.

Here is the [Seifert-matrix presentation of the Alexander module](../../../../../seifert-matrix-presentation-of-the-alexander-module.md) with its topological justification. Cut X along F, obtaining a connected manifold Y with two boundary copies $F^+$ and $F^-$. Up to collars this is the complement of a thickening of F in $S^3$. [Alexander duality](../../../../../alexander-duality.md) gives $H_1(Y;\mathbb Z)\cong\mathbb Z^{2g}$ and the perfect linking pairing with $H_1(F;\mathbb Z)$. Choose generators $b_j$ satisfying $\operatorname{lk}(b_j,a_i)=\delta_{ij}$. This [homology](../../../../../homology-split.md) statement does not require Y to be a handlebody. The two inclusions satisfy

$$
i_+(a_i)=\sum_jV_{ij}b_j,\qquad i_-(a_i)=\sum_jV_{ji}b_j.
$$

Indeed the first coefficients are the defining positive [linking numbers](../../../../../linking-number.md); for the second, moving the two curves to opposite sides and using symmetry of linking gives $\operatorname{lk}(a_i^-,a_j)=\operatorname{lk}(a_j^+,a_i)$.

Stack copies of Y, identifying the positive copy of F in one layer with the negative copy in the next. This is $\widetilde X$. The [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md), with all translates collected into Laurent [modules](../../../../../module-mathematics.md), contains

$$
H_1(F)\otimes\Lambda\xrightarrow{\,t i_+-i_-\,}H_1(Y)\otimes\Lambda\longrightarrow\mathcal A_K\longrightarrow H_0(F)\otimes\Lambda\xrightarrow{\,t-1\,}H_0(Y)\otimes\Lambda.
$$

The last map is injective because $\Lambda$ is an [integral domain](../../../../../integral-domain.md). Thus the entire [Alexander module](../../../../../alexander-module-of-a-knot.md) is presented by the row relations $tV-V^T$ (transpose the [matrix](../../../../../matrix.md) if using column vectors). At $t=1$ its [determinant](../../../../../determinant.md) is $\det(V-V^T)=1$, so the [determinant](../../../../../determinant.md) is nonzero and the [module](../../../../../module-mathematics.md) is torsion. Consequently

$$
\boxed{\Delta_K(t)\doteq\det(tV-V^T),\qquad\operatorname{br}\Delta_K\leq2g_s(K),}
$$

where $\doteq$ denotes equality up to a Laurent unit. The second conclusion follows because a [determinant](../../../../../determinant.md) of size $2g$ with entries linear in t has breadth at most $2g$; minimize over [Seifert surfaces](../../../../../seifert-surface.md).

For the displayed [knot](../../../../../knot.md) we give a reproducible diagram calculation. Label its ten crossings A through J as follows: A and B are the two upper crossings from left to right; C,D,E are the next three crossings in descending order; F is the crossing below E on the almost vertical strand; G is the left crossing of the bottom loop; H,I,J are the remaining three bottom crossings from left to right. With one traversal direction the over/under record is

$$
A_O\ B_U\ J_O\ I_U\ H_O\ F_U\ G_O\ H_U\ I_O\ J_U\ D_O\ C_U\ E_O\ D_U\ B_O\ A_U\ C_O\ E_U\ F_O\ G_U.
$$

The crossings have the same sign. Choose the meridian/deck convention giving the conjugation relation below; the opposite convention replaces t by $t^{-1}$ and gives the same reciprocal [polynomial](../../../../../polynomial-split.md) up to a unit.

Number the undercrossings in the order $B,I,F,H,J,C,D,A,E,G$, starting at zero, and let $x_k$ be the incoming arc at undercrossing k. The overpassing arc numbers are

$$
(o_0,\ldots,o_9)=(7,4,9,2,1,8,5,0,6,3).
$$

The [Wirtinger presentation](../../../../../wirtinger-presentation.md) has $x_{k+1}=x_{o_k}x_kx_{o_k}^{-1}$, with indices modulo ten. Its lifted cellular boundaries, or equivalently [Fox derivatives](../../../../../fox-derivative.md), give the Alexander relation [matrix](../../../../../matrix.md)

$$
M_{kj}=t\delta_{j,k}-\delta_{j,k+1}+(1-t)\delta_{j,o_k}.
$$

Delete the redundant final relation and the last column: the resulting [matrix](../../../../../matrix.md) presents the [Alexander module](../../../../../alexander-module-of-a-knot.md) on the nine relative arc generators. To make the [determinant](../../../../../determinant.md) check transparent, set $h=2t^2-3t+2$, $k=4t^2-7t+5$, and $\ell=2t^2-2t+1$. Eliminating unit pivots reduces this nine-generator presentation to

$$
N=\begin{pmatrix}th+(1-t)^2k&-h\\t(1-t)k&\ell\end{pmatrix}.
$$

For example, writing the relative generators as $z_0,\ldots,z_8$, the eliminated relations give $z_3=tz_2$, $z_4=(t^2-t+1)z_2$, $z_1=(t^2-2t+2)z_2$, $z_5=hz_2$, $z_7=(1-t)hz_2+tz_6$, $z_0=t^{-1}(t^2-2t+2-(1-t)^2h)z_2-(1-t)z_6$, and $z_8=(1-t)kz_2+(2t-1)z_6$. The two remaining relations are precisely the rows of N. Hence

$$
\boxed{\Delta_K(t)\doteq\det N=5t^4-15t^3+21t^2-15t+5.}
$$

As a second [determinant](../../../../../determinant.md) check, the unreduced nine-by-nine cofactor of M is $t^2\det N$. The [polynomial](../../../../../polynomial-split.md) has value one at $t=1$ and is reciprocal, as required.

For the genus upper bound, the oriented smoothing has seven [Seifert circles](../../../../../seifert-circle.md). This can also be checked from the traversal record: number its twenty entries starting at one; smoothing sends an incoming visit to the entry following its other visit to the same crossing. The cycles are $(1,17,13,19,7)$, $(2,16)$, $(3,11,15)$, $(4,10)$, $(5,9)$, $(6,20,8)$, and $(12,18,14)$. The [Seifert algorithm](../../../../../seifert-algorithm.md) therefore gives seven disks and ten bands, so $\chi(F)=7-10=-3=1-2g(F)$ and $g(F)=2$. The Alexander breadth is four, so the [Alexander breadth bound on Seifert genus](../../../../../alexander-breadth-bound-on-seifert-genus.md) gives the matching lower bound. Thus $\boxed{g_s(K)=2}$.

Finally, modulo two the primitive [polynomial](../../../../../polynomial-split.md) becomes $t^4+t^3+t^2+t+1$. It has neither zero nor one as a root. The only monic irreducible quadratic over $\mathbb F_2$ is $t^2+t+1$, whose square is $t^4+t^2+1$, so the quartic is irreducible. Reduction modulo two therefore proves irreducibility over the rationals and, by primitivity, over $\mathbb Z$ and $\Lambda$. If K were a sum of two nontrivial [knots](../../../../../knot.md), [additivity of Seifert genus](../../../../../additivity-of-seifert-genus.md) would force both summands to have genus one. Their Alexander [polynomials](../../../../../polynomial-split.md) multiply, so irreducibility would make one [polynomial](../../../../../polynomial-split.md) a unit and the other equal to this breadth-four [polynomial](../../../../../polynomial-split.md), contradicting the breadth-at-most-two bound for genus one. This uses the [full-degree irreducible Alexander polynomial implies a prime knot](../../../../../full-degree-irreducible-alexander-polynomial-implies-a-prime-knot.md) criterion, rather than irreducibility alone. Therefore **K is prime**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
