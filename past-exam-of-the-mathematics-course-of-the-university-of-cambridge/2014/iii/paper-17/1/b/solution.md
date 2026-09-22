<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Dolbeault theorem](../../../../../../dolbeault-theorem.md) identifies

$$
 \boxed{H_{\bar\partial}^{p,q}(X)\cong\check H^q(X,\Omega_X^p),}
$$

where $\Omega_X^p$ is the [sheaf](../../../../../../sheaf-mathematics.md) of [holomorphic differential forms](../../../../../../holomorphic-differential-form.md) of degree $p$.

The local analytic ingredient is the [Dolbeault-Poincaré lemma](../../../../../../dolbeault-poincare-lemma.md): a $\bar\partial$-closed smooth $(p,q)$-form with $q>0$ is locally $\bar\partial$-exact. Here is a local proof. On a polydisc, the one-variable [Cauchy-Green operator](../../../../../../cauchy-green-operator.md) in coordinate $z_j$ is

$$
 (T_jg)(z)=\frac1\pi\int_{\mathbb C}
 \frac{\chi(\zeta)g(z_1,\ldots,\zeta,\ldots,z_m)}{z_j-\zeta}\,dA(\zeta),
$$

with a smooth cutoff supported in the coordinate disc and equal to one on a smaller disc. The fundamental-solution identity $\partial_{\bar z}(1/(\pi z))=\delta_0$ gives $\partial_{\bar z_j}T_jg=g$ on that smaller disc. The operator is smooth in the parameters and commutes with derivatives in the other coordinates.

For a $(0,q)$-form, write $\alpha=d\bar z_m\wedge\beta+\gamma$, with neither $\beta$ nor $\gamma$ containing $d\bar z_m$. Subtract $\bar\partial(T_m\beta)$. The remainder contains no $d\bar z_m$, remains closed, and its coefficients are holomorphic in $z_m$. Repeat with $z_{m-1}$ and then the other coordinates, shrinking discs as needed. Each new integral preserves the holomorphic dependence already achieved. At the end the closed remainder has positive antiholomorphic degree but contains no antiholomorphic differential, so it is zero. Factoring out each holomorphic basis form $dz_I$ gives the same assertion for $(p,q)$-forms, with the fixed degree sign included in the primitive. At degree zero, the kernel of $\bar\partial$ consists precisely of holomorphic coefficients.

Thus the following is an exact [Dolbeault resolution of holomorphic differential forms](../../../../../../dolbeault-resolution-of-holomorphic-differential-forms.md) of [sheaves](../../../../../../sheaf-mathematics.md):

$$
 0\longrightarrow\Omega_X^p\longrightarrow\mathcal A^{p,0}
 \xrightarrow{\bar\partial}\mathcal A^{p,1}\xrightarrow{\bar\partial}\cdots
 \xrightarrow{\bar\partial}\mathcal A^{p,m}\longrightarrow0.
$$

Each [sheaf](../../../../../../sheaf-mathematics.md) of smooth forms is a [fine sheaf](../../../../../../fine-sheaf.md): multiplication by a smooth [partition of unity](../../../../../../partition-of-unity.md) supplies endomorphisms supported in its open cover. [Fine sheaves](../../../../../../fine-sheaf.md) on a paracompact manifold have zero positive [sheaf cohomology](../../../../../../sheaf-cohomology.md); the Čech contraction sums a cochain against the [partition of unity](../../../../../../partition-of-unity.md), giving $\delta h+h\delta=I$ in positive degrees. The general [acyclic resolution theorem](../../../../../../acyclic-resolution-theorem.md) therefore computes $\check H^q(X,\Omega_X^p)$ as the cohomology of the global-section complex above. That complex is exactly the [Dolbeault resolution of holomorphic differential forms](../../../../../../dolbeault-resolution-of-holomorphic-differential-forms.md), proving the claimed isomorphism. The sheaf-cohomology/Čech comparison and the acyclic-resolution principle are the stated general Čech properties used here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
