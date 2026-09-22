<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [principal bundle](../../../../../principal-bundle.md) separates the geometry of internal symmetry from a chosen local [gauge potential](../../../../../gauge-field.md). Let $\pi:P\to X$ be a principal $G$-bundle with a free right [Lie group action](../../../../../lie-group-action.md). Each fiber is a copy of $G$, but generally no single identification works globally. A [principal connection](../../../../../connection-principal-bundle.md) tells us how to compare fibers over nearby base points. Its physical interpretation is a prescription for [parallel transport](../../../../../parallel-transport.md) of internal states.

For $\xi\in\mathfrak g$, the vertical [fundamental vector field](../../../../../fundamental-vector-field.md) is $\xi^\#_p=\left.\frac d{ds}\right|_0p\exp(s\xi)$. A [principal connection](../../../../../connection-principal-bundle.md) is a [Lie algebra](../../../../../lie-algebra-split.md)-valued one-form $\mathcal A$ on $P$ satisfying

$$
\boxed{\mathcal A(\xi^\#)=\xi,\qquad R_g^*\mathcal A=\operatorname{Ad}_{g^{-1}}\mathcal A.}
$$

Equivalently, the [horizontal distribution of a principal connection](../../../../../horizontal-distribution-of-a-principal-connection.md) $H_p=\ker\mathcal A_p$ complements the vertical tangent space and is preserved by right translation. Given a curve in $X$ and an initial point in its fiber, there is a unique horizontal lift. For a closed curve its endpoint differs from its start by a group element: the [holonomy of a connection](../../../../../holonomy.md). Thus a [principal connection](../../../../../connection-principal-bundle.md) contains both infinitesimal and global transport information.

Choose local sections $s_\alpha:U_\alpha\to P$. Their [local principal connection forms](../../../../../local-principal-connection-form.md) $A_\alpha=s_\alpha^*\mathcal A$ are the usual [gauge potentials](../../../../../gauge-field.md). If $s_\beta=s_\alpha g_{\alpha\beta}$ on an overlap, equivariance and reproduction of vertical generators give

$$
\boxed{A_\beta=g_{\alpha\beta}^{-1}A_\alpha g_{\alpha\beta}
+g_{\alpha\beta}^{-1}dg_{\alpha\beta}.}
$$

This inhomogeneous law means that a [gauge potential](../../../../../gauge-field.md) is not an ordinary globally defined tensor. Its local formulas glue to a global [principal connection](../../../../../connection-principal-bundle.md). The same law describes changing a local section by a gauge function. For example, to impose [temporal gauge](../../../../../temporal-gauge.md) locally, solve $\partial_tg=-A_tg$ so the transformed time component vanishes.

The [curvature of a principal connection](../../../../../curvature-of-a-principal-connection.md) is

$$
\boxed{\mathcal F=d\mathcal A+\frac12[\mathcal A\wedge\mathcal A],\qquad
F_\alpha=dA_\alpha+A_\alpha\wedge A_\alpha.}
$$

Unlike the [principal connection](../../../../../connection-principal-bundle.md) form, its curvature is horizontal and equivariant. Consequently $F_\beta=g_{\alpha\beta}^{-1}F_\alpha g_{\alpha\beta}$, and the [gauge curvature](../../../../../gauge-field-strength.md) is globally a two-form on $X$ with values in the [adjoint bundle](../../../../../adjoint-bundle.md) $\operatorname{ad}P=P\times_{\operatorname{Ad}}\mathfrak g$. The curvature measures the failure of horizontal directions to close under brackets: for horizontal lifts $U,V$, $\mathcal F(U,V)=-\mathcal A([U,V])$. A [flat principal connection](../../../../../flat-principal-connection.md) has an integrable horizontal distribution, although nontrivial global [holonomy of a connection](../../../../../holonomy.md) can remain around noncontractible curves.

The [covariant exterior derivative](../../../../../exterior-covariant-derivative.md) on [adjoint bundle](../../../../../adjoint-bundle.md)-valued forms is locally $D_A=d+[A,\,\cdot\,]$. Expanding $F=dA+A\wedge A$ and using $d^2=0$ yields the [Bianchi identity](../../../../../bianchi-identity.md)

$$
\boxed{D_AF=0.}
$$

For a representation $\rho$ of $G$, the same [principal connection](../../../../../connection-principal-bundle.md) induces transport in the corresponding [associated vector bundle](../../../../../associated-vector-bundle.md); locally its [covariant derivative](../../../../../covariant-derivative.md) is $d+\rho_*(A)$. This explains why charged matter and the [gauge curvature](../../../../../gauge-field-strength.md) use the same [gauge potential](../../../../../gauge-field.md).

Now put an oriented [Riemannian metric](../../../../../riemannian-metric.md) on a four-dimensional base and take $G=SU(n)$. Use anti-Hermitian matrices with positive pairing $-\operatorname{tr}(XY)$, as in the preceding solution. The [Yang-Mills action](../../../../../yang-mills-action.md) is

$$
S[A]=-\frac1{g_{\mathrm{YM}}^2}\int_X\operatorname{tr}(F\wedge*F).
$$

Its gauge invariance follows from curvature conjugation and invariance of the [trace](../../../../../matrix-trace.md). Under a compactly supported variation $a=\delta A$, $\delta F=D_Aa$. Integration by parts therefore gives

$$
\delta S=-\frac2{g_{\mathrm{YM}}^2}\int_X\operatorname{tr}(a\wedge D_A*F),\qquad
\boxed{D_A*F=0.}
$$

This is a second-order equation for the [gauge potential](../../../../../gauge-field.md). The [self-dual Yang-Mills equations](../../../../../self-dual-yang-mills-equations.md) $F=*F$ and the [Anti-self-dual Yang-Mills equations](../../../../../anti-self-dual-yang-mills-equations.md) $F=-*F$ are first-order equations. Either implies the full [Yang-Mills equations](../../../../../yang-mills-equations.md) immediately, since $D_A*F=\pm D_AF=0$ by the [Bianchi identity](../../../../../bianchi-identity.md). This is [self-duality implies Yang-Mills equations](../../../../../self-duality-implies-yang-mills-equations.md).

A [Yang-Mills instanton](../../../../../yang-mills-instanton.md) is a smooth finite-action Euclidean solution with self-dual or anti-self-dual [gauge curvature](../../../../../gauge-field-strength.md). Its defining first-order condition depends on the [principal connection](../../../../../connection-principal-bundle.md), the metric and the orientation. Since the [Hodge star operator](../../../../../hodge-star-operator.md) on two-forms is unchanged under $g\mapsto e^{2f}g$ in four dimensions, self-duality and the [Yang-Mills action](../../../../../yang-mills-action.md) are conformally invariant. In particular Euclidean solutions can be studied through conformal compactification, with appropriate behavior at infinity.

The global topology is encoded by [Chern-Weil theory](../../../../../chern-weil-homomorphism.md). Since $\operatorname{tr}F=0$, the [Second Chern form](../../../../../second-chern-form.md) and [Second Chern number](../../../../../second-chern-number.md) are

$$
c_2(A)=\frac1{8\pi^2}\operatorname{tr}(F\wedge F),\qquad
k=\int_Xc_2(A)\in\mathbb Z
$$

on a compact oriented four-manifold. The [Bianchi identity](../../../../../bianchi-identity.md) makes $c_2(A)$ closed. More explicitly, under a connection variation,

$$
\delta\operatorname{tr}(F\wedge F)
=2\operatorname{tr}(D_Aa\wedge F)
=2d\operatorname{tr}(a\wedge F).
$$

Thus the integrated [Second Chern number](../../../../../second-chern-number.md) is independent of the [principal connection](../../../../../connection-principal-bundle.md) on a fixed bundle, with the usual fixed-boundary condition on a noncompact base. The space of connections is affine, so integrating this variation along a straight path also proves that their characteristic forms differ by an exact form.

Locally the same characteristic form has a [Chern-Simons 3-form](../../../../../chern-simons-3-form.md) primitive:

$$
\operatorname{tr}(F\wedge F)=d\operatorname{tr}\left(A\wedge dA+\frac23A\wedge A\wedge A\right).
$$

On $\mathbb R^4$ the underlying bundle is trivial, but a finite-action instanton with the standard extendible behavior at infinity can define a nontrivial bundle after adding the point at infinity. The transition map on an equatorial $S^3$ takes values in $SU(n)$; for $n\ge2$, its homotopy class lies in $\pi_3(SU(n))\cong\mathbb Z$. The boundary integral of the [Chern-Simons 3-form](../../../../../chern-simons-3-form.md) computes that integer with the chosen sign convention. This reconciles a local matrix-valued [gauge potential](../../../../../gauge-field.md) on $\mathbb R^4$ with nonzero global [Second Chern number](../../../../../second-chern-number.md) on $S^4$.

Finally the [Hodge splitting of Euclidean two-forms](../../../../../hodge-splitting-of-euclidean-two-forms.md) produces the [Yang-Mills instanton Bogomolny bound](../../../../../yang-mills-instanton-bogomolny-bound.md)

$$
\boxed{S[A]\ge\frac{8\pi^2}{g_{\mathrm{YM}}^2}|k|.}
$$

Equality holds exactly when the opposite-duality component of the [gauge curvature](../../../../../gauge-field-strength.md) vanishes. Thus a [Yang-Mills instanton](../../../../../yang-mills-instanton.md) is an **absolute action minimum in its fixed topological sector**, not merely a stationary solution. In this trace convention self-dual instantons have $k<0$ and anti-self-dual instantons have $k>0$. In the zero sector, a self-dual or anti-self-dual finite-action solution has $S=0$ and hence $F=0$.

Different [principal connections](../../../../../connection-principal-bundle.md) related by bundle gauge transformations describe the same physical configuration. Fixing $k$ and taking the quotient of instanton solutions by this [gauge equivalence of principal connections](../../../../../gauge-equivalence-of-principal-connections.md) gives the [instanton moduli space](../../../../../instanton-moduli-space.md). Near an anti-self-dual solution, write a variation as $a\in\Omega^1(X,\operatorname{ad}P)$. The linearized instanton equation and infinitesimal gauge transformations are

$$
P_+D_Aa=0,\qquad a\sim a+D_A\varepsilon.
$$

A local gauge condition $D_A^*a=0$ removes this redundancy. The combined operator $D_A^*\oplus P_+D_A$ is elliptic: for nonzero covector $\xi$, its principal symbol $a\mapsto(\iota_{\xi^\sharp}a,P_+(\xi\wedge a))$ has zero kernel. Choose $\xi=dt$; the first component removes $a_t$, and the self-dual projection of $dt\wedge a$ removes the three remaining components. This connects the [instanton moduli space](../../../../../instanton-moduli-space.md) to geometric analysis, while the characteristic number and transport law explain its topological and physical meaning.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
