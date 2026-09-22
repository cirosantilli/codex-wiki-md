<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the given orientation throughout, and the usual convention that the manifold has no boundary. In an oriented [manifold chart](../../../../../manifold-chart.md) the [metric volume form](../../../../../metric-volume-form.md) is

$$
\omega_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

If $y$ is another oriented chart and $A=\partial x/\partial y$, then $g_y=A^tg_xA$, so $\sqrt{\det g_y}=(\det A)\sqrt{\det g_x}$ because $\det A>0$. This is exactly the transformation of the top [exterior product](../../../../../exterior-product.md). The formulas therefore agree on overlaps and define a smooth positive [volume form](../../../../../volume-form.md). Equivalently it takes value one on any positively oriented orthonormal tangent frame.

The metric induces an [inner product](../../../../../inner-product.md) on $p$-forms by making the increasing exterior products of an orthonormal coframe orthonormal. The [Hodge star operator](../../../../../hodge-star-operator.md) is the unique pointwise linear map $*:\Lambda^pT^*M\to\Lambda^{n-p}T^*M$ satisfying

$$
\eta\wedge *\theta=\langle\eta,\theta\rangle_g\omega_g.
$$

For an increasing multi-index $I$, $*e^I$ is the complementary wedge with the sign making $e^I\wedge *e^I=\omega_g$. Swapping the blocks of $p$ and $n-p$ factors introduces $(-1)^{p(n-p)}$. Therefore

$$
\boxed{*^2=(-1)^{p(n-p)}\operatorname{id}\quad\text{on }\Omega^p(M).}
$$

In particular $*1=\omega_g$ and $*\omega_g=1$.

For compactly supported smooth $f$, the $(n-1)$-form $f*\alpha$ has compact support. [Stokes theorem](../../../../../stokes-theorem.md) and the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) give

$$
0=\int_Md(f*\alpha)=\int_Mdf\wedge *\alpha+\int_Mf\,d*\alpha.
$$

A top form $\tau$ equals $(*\tau)\omega_g$. Consequently this [Hodge integration by parts for one-forms](../../../../../hodge-integration-by-parts-for-one-forms.md) becomes exactly

$$
\int_M(-f*d*\alpha)\omega_g=\int_M\langle df,\alpha\rangle_g\omega_g.
$$

Compact support of $f$ is enough; $\alpha$ need not itself have compact support.

Define the [codifferential](../../../../../codifferential.md) on $p$-forms by $\delta=(-1)^{n(p+1)+1}*d*$ and the [Hodge Laplacian](../../../../../hodge-laplacian.md) by $\Delta=d\delta+\delta d$. A [harmonic differential form](../../../../../harmonic-differential-form.md) is a smooth form in $\ker\Delta$. On functions this is the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md), $\Delta f=\delta df=-\operatorname{div}_g\operatorname{grad}_gf$. This sign convention is required by the product identity; it is the negative of the $\operatorname{div}\operatorname{grad}$ convention also commonly used for the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md).

For a $p$-form $\beta$, the square of the [Hodge star operator](../../../../../hodge-star-operator.md) and the [codifferential](../../../../../codifferential.md) formula give

$$
\delta(*\beta)=(-1)^{p+1}*d\beta,\qquad d(*\beta)=(-1)^p*\delta\beta.
$$

Applying the second formula to $d\beta$ and the first to $\delta\beta$ gives

$$
\Delta(*\beta)=(-1)^{p+1}d(*d\beta)+(-1)^p\delta(*\delta\beta)=*\delta d\beta+*d\delta\beta=*\Delta\beta.
$$

Thus [Hodge star commutes with the Hodge Laplacian](../../../../../hodge-star-commutes-with-the-hodge-laplacian.md). Since $*$ is invertible, **$\beta$ is harmonic if and only if $*\beta$ is harmonic.** This holds without compactness; we have not used the generally false noncompact implication that a harmonic form must be closed and coclosed.

For a smooth function $h$ and one-form $\alpha$, the same [graded Leibniz rule](../../../../../graded-leibniz-rule.md) gives $\delta(h\alpha)=h\delta\alpha-*\,(dh\wedge *\alpha)=h\delta\alpha-\langle dh,\alpha\rangle_g$. Apply this to $d(f_1f_2)=f_2df_1+f_1df_2$ to obtain the [product rule for the positive Laplace-Beltrami operator](../../../../../product-rule-for-the-positive-laplace-beltrami-operator.md)

$$
\boxed{\Delta(f_1f_2)=f_2\Delta f_1+f_1\Delta f_2-2\langle df_1,df_2\rangle_g.}
$$

The [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) states that on a compact oriented boundaryless [Riemannian manifold](../../../../../riemannian-manifold.md), smooth forms have the $L^2$-orthogonal decomposition

$$
\Omega^p(M)=\mathcal H^p(M)\oplus d\Omega^{p-1}(M)\oplus\delta\Omega^{p+1}(M),\qquad\mathcal H^p(M)=\ker\Delta,
$$

and each [de Rham cohomology](../../../../../de-rham-cohomology.md) class has a unique [harmonic differential form](../../../../../harmonic-differential-form.md) representative. To spell out the last conclusion, a harmonic form is closed and coclosed because $\langle\Delta\eta,\eta\rangle=\|d\eta\|^2+\|\delta\eta\|^2$. If a closed form decomposes as $h+du+\delta v$, then $d\delta v=0$; integration by parts gives $\|\delta v\|^2=\langle v,d\delta v\rangle=0$. Thus it represents $h$. A harmonic exact form has zero norm by adjointness, proving uniqueness. The analytic existence of the decomposition is the stated [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md).

Now let $M$ be compact, connected and oriented. A harmonic function satisfies $0=\langle f,\Delta f\rangle=\|df\|^2$, so it is constant. The [Hodge star operator](../../../../../hodge-star-operator.md) identifies $\mathcal H^0(M)$ with $\mathcal H^n(M)$, hence $\mathcal H^n(M)=\mathbb R\omega_g$. A [Riemannian metric](../../../../../riemannian-metric.md) exists by Question 3 even if none was initially chosen. Using the harmonic representative of each class, we obtain the [top de Rham cohomology of a compact connected oriented manifold](../../../../../top-de-rham-cohomology-of-a-compact-connected-oriented-manifold.md)

$$
\boxed{H^n_{\mathrm{dR}}(M)\cong\mathbb R,\qquad[\omega_g]\text{ spans it}.}
$$

The class is nonzero also directly from [Stokes theorem](../../../../../stokes-theorem.md), since $\int_M\omega_g>0$ while every exact top form has zero integral. Boundarylessness matters: a compact interval has zero first [de Rham cohomology](../../../../../de-rham-cohomology.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
