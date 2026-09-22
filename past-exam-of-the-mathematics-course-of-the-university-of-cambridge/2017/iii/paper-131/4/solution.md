<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

At each point, use the inverse metric on the cotangent space. It induces an [inner product](../../../../../inner-product.md) on $p$-forms by

$$
\langle\xi_1\wedge\cdots\wedge\xi_p,\eta_1\wedge\cdots\wedge\eta_p\rangle
=\det\bigl(g^{-1}(\xi_i,\eta_j)\bigr).
$$

Equivalently, wedges of distinct members of an orthonormal coframe form an [orthonormal basis](../../../../../orthonormal-basis.md). Choose an [orientation](../../../../../orientation-of-a-simplex.md) to define the ordinary global [Hodge star operator](../../../../../hodge-star-operator.md) by $\alpha\wedge*\beta=\langle\alpha,\beta\rangle\,d\mathrm{vol}_g$. It maps $p$-forms to $(n-p)$-forms and obeys $*^2=(-1)^{p(n-p)}$. We use real forms; complex forms are obtained by complex-linear extension. Without an [orientation](../../../../../orientation-of-a-simplex.md) an ordinary global star is not available without twisting the target, so [orientation](../../../../../orientation-of-a-simplex.md) is implicit in this first part.

With the [codifferential](../../../../../codifferential.md) $\delta_p=(-1)^{n(p+1)+1}*d*$ for $p>0$ and $\delta_0=0$, define the [Hodge Laplacian](../../../../../hodge-laplacian.md) $\Delta=d\delta+\delta d$. On functions it is the nonnegative-sign [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md), $\Delta f=-\operatorname{div}\operatorname{grad}f$. A [harmonic differential form](../../../../../harmonic-differential-form.md) satisfies $\Delta\alpha=0$.

For $\alpha$ of degree $p$, the displayed sign formula and star square give

$$
d(*\alpha)=(-1)^p*\delta\alpha,\qquad
\delta(*\alpha)=(-1)^{p+1}*d\alpha.
$$

Applying the identities again, at degrees $p-1$ and $p+1$, proves the [Hodge star commutes with the Hodge Laplacian](../../../../../hodge-star-commutes-with-the-hodge-laplacian.md) relation

$$
\boxed{\Delta(*\alpha)=*\Delta\alpha.}
$$

Since star is invertible, $\alpha$ is harmonic if and only if $*\alpha$ is harmonic. This part does not need compactness; zero-degree and top-degree terms are interpreted as zero when their degrees are outside the range.

For the remaining cohomological statements assume a compact oriented manifold without boundary. The [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) gives the $L^2$-orthogonal decomposition

$$
\Omega^p(M)=\mathcal H^p(M)\oplus d\Omega^{p-1}(M)\oplus\delta\Omega^{p+1}(M),
$$

where $\mathcal H^p=\ker\Delta$ is finite-dimensional and consists of smooth forms. Formal adjointness gives $\langle\Delta\alpha,\alpha\rangle_{L^2}=\|d\alpha\|_{L^2}^2+\|\delta\alpha\|_{L^2}^2$, so [harmonic differential forms](../../../../../harmonic-differential-form.md) are [closed differential forms](../../../../../closed-differential-form.md) and [coclosed differential forms](../../../../../coclosed-differential-form.md).

If $\Delta f\ge0$, formal adjointness and $\Delta1=0$ give $\int_M\Delta f=0$. A continuous nonnegative function with zero integral vanishes, so $\Delta f=0$. Then $\|df\|_{L^2}^2=\langle\Delta f,f\rangle=0$. Thus the [a function with nonnegative Laplacian on a closed manifold is locally constant](../../../../../a-function-with-nonnegative-laplacian-on-a-closed-manifold-is-locally-constant.md) assertion is

$$
\boxed{df=0,\qquad f\text{ is constant on each connected component}.}
$$

It is globally constant when $M$ is connected. The PDF does not explicitly include connectedness here; on two disjoint circles one may take different constants, so literal global constancy needs that qualification. Boundaryless is the standard manifold convention in this argument; otherwise boundary conditions are necessary.

For a [closed differential form](../../../../../closed-differential-form.md) $\alpha$, write its Hodge decomposition as $\alpha=h+d\beta+\delta\gamma$. Since $d\alpha=dh=0$, we have $d\delta\gamma=0$. Formal adjointness yields $\|\delta\gamma\|^2=\langle\gamma,d\delta\gamma\rangle=0$, so $\alpha=h+d\beta$. Thus $h$ represents its [de Rham cohomology](../../../../../de-rham-cohomology.md) class. If two harmonic representatives differ by $d\beta$, their difference $h$ has $\|h\|^2=\langle d\beta,h\rangle=\langle\beta,\delta h\rangle=0$. Therefore

$$
\boxed{\mathcal H^p(M)\cong H^p_{\mathrm{dR}}(M),\quad\text{with a unique harmonic representative in each class}.}
$$

Finally let $h\in G$. A connected [Lie group](../../../../../lie-group.md) admits a smooth path $h_t$ from the identity to $h$. The maps $R_{h_t}$ give a smooth homotopy between the identity and $R_h$. The [homotopy invariance of de Rham cohomology](../../../../../homotopy-invariance-of-de-rham-cohomology.md) says their pullbacks agree on cohomology. The maps $R_{h_t}$ preserve [orientation](../../../../../orientation-of-a-simplex.md), since their Jacobian signs cannot change from the identity along the path. As an orientation-preserving isometry, $R_h$ commutes on forms with star, exterior differentiation, codifferentiation and consequently the [Hodge Laplacian](../../../../../hodge-laplacian.md). Hence $R_h^*\alpha$ is harmonic and represents the same cohomology class as a harmonic $\alpha$. Uniqueness now proves the [harmonic forms are fixed by a connected isometric group action](../../../../../harmonic-forms-are-fixed-by-a-connected-isometric-group-action.md) conclusion

$$
\boxed{R_h^*\alpha=\alpha\qquad(h\in G).}
$$

The argument also applies componentwise when $M$ is disconnected.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 131](../../paper-131-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
