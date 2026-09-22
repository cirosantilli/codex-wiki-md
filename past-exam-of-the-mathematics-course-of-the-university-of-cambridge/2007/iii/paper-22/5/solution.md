<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $n=\dim_{\mathbb C}X$, and use the complex orientation. Write $g$ for the real [Riemannian metric](../../../../../riemannian-metric.md) underlying the [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md). Its [fundamental form of a Hermitian manifold](../../../../../fundamental-form-of-a-hermitian-manifold.md) is

$$
\omega(u,v)=g(Ju,v),\qquad
\omega=\frac{i}{2}\sum_{a,b}h_{a\bar b}\,dz^a\wedge d\bar z^b,
$$

where $g=\operatorname{Re}(\sum h_{a\bar b}\,dz^a\otimes d\bar z^b)$ in this convention. It is real and of type $(1,1)$, since $g(Ju,Jv)=g(u,v)$. Choose an adapted real orthonormal frame $E_j,F_j=JE_j$ and its dual coframe $e^j,f^j$. Then $\omega=\sum_j e^j\wedge f^j$, giving the [Riemannian volume form](../../../../../riemannian-volume-form.md)

$$
\boxed{\operatorname{vol}_g=e^1\wedge f^1\wedge\cdots\wedge e^n\wedge f^n=\frac{\omega^n}{n!}.}
$$

We use the complex-linear [Hodge star operator](../../../../../hodge-star-operator.md), the extension of the real metric star characterized on equal-degree forms by

$$
\alpha\wedge *\overline\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g.
$$

It maps $(p,q)$-forms to $(n-q,n-p)$-forms and satisfies $**\alpha=(-1)^{p+q}\alpha$. It is distinct from the conjugate-linear map $\alpha\mapsto*\overline\alpha$. In the adapted coframe the star of $e^j\wedge f^j$ is the wedge product of all the other two-dimensional factors, with positive sign. Summing proves the [Hodge star of the fundamental Hermitian form](../../../../../hodge-star-of-the-fundamental-hermitian-form.md) formula

$$
\boxed{*\omega=\frac{\omega^{n-1}}{(n-1)!}.}
$$

This computation uses no closedness assumption on $\omega$.

Use the integrated Hermitian inner product $(\alpha,\beta)=\int_X\alpha\wedge*\overline\beta$. The [formal adjoints](../../../../../formal-adjoint.md) $d^*$ and $\bar\partial^*$ are defined by $(d\alpha,\beta)=(\alpha,d^*\beta)$ and $(\bar\partial\alpha,\beta)=(\alpha,\bar\partial^*\beta)$; compact manifolds here have no boundary. The [Hodge Laplacian](../../../../../hodge-laplacian.md) and [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) are

$$
\Delta_d=dd^*+d^*d,\qquad
\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.
$$

The [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) states that

$$
\mathcal A^{p,q}(X)=\mathcal H_{\bar\partial}^{p,q}\oplus
\bar\partial\mathcal A^{p,q-1}(X)\oplus
\bar\partial^*\mathcal A^{p,q+1}(X)
$$

is an orthogonal direct sum, with finite-dimensional $\mathcal H_{\bar\partial}^{p,q}=\ker\Delta_{\bar\partial}$. Each [Dolbeault cohomology](../../../../../dolbeault-cohomology.md) class

$$
H_{\bar\partial}^{p,q}(X)=\ker(\bar\partial:\mathcal A^{p,q}\to\mathcal A^{p,q+1})/\bar\partial\mathcal A^{p,q-1}
$$

has a unique representative in $\mathcal H_{\bar\partial}^{p,q}$. A form is harmonic exactly when both $\bar\partial\alpha$ and $\bar\partial^*\alpha$ vanish, since its Laplacian inner product is the sum of their squared norms.

Now let $L\alpha=\omega\wedge\alpha$ be the [Hermitian Lefschetz operator](../../../../../lefschetz-operator-on-a-hermitian-manifold.md) and let $\Lambda$ be its pointwise adjoint. For $\beta$ of total degree $r=p+q$ and $\alpha$ of degree $r-2$, the defining inner products give

$$
(L\alpha)\wedge*\overline\beta
=\alpha\wedge\omega\wedge*\overline\beta
=\alpha\wedge*\overline{\Lambda\beta}.
$$

The wedge pairing is nondegenerate, so $*\overline{\Lambda\beta}=L*\overline\beta$. Apply another star to the degree-$(r-2)$ form and use that the star and $L$ commute with conjugation. This yields

$$
\boxed{\Lambda\beta=(-1)^{r-2}*L*\beta=(-1)^{p+q}*L*\beta.}
$$

For degrees below two both sides vanish. The argument also identifies its bidegree as $(-1,-1)$ and does not require the [Kähler](../../../../../kahler-manifold.md) condition.

Assume now that $d\omega=0$, so the metric is a [Kähler metric](../../../../../kahler-metric.md). Start with the supplied [Kähler identities](../../../../../kahler-identities.md) relation $[\Lambda,\partial]=i\bar\partial^*$. Since $\Lambda$ is real, conjugation gives $[\Lambda,\bar\partial]=-i\partial^*$, hence

$$
\bar\partial^*=-i[\Lambda,\partial],\qquad
\partial^*=i[\Lambda,\bar\partial].
$$

The commutators are ordinary commutators because $\Lambda$ has even degree. Using $\partial^2=0$ we obtain, by direct expansion,

$$
\partial\bar\partial^*+\bar\partial^*\partial
=-i\left(\partial\Lambda\partial-\partial^2\Lambda+\Lambda\partial^2-\partial\Lambda\partial\right)=0.
$$

Conjugation gives $\bar\partial\partial^*+\partial^*\bar\partial=0$ as well. Expanding the two unmixed Laplacians and using $\partial\bar\partial=-\bar\partial\partial$ gives the same operator:

$$
\begin{aligned}
\Delta_\partial
&=i\left(\partial\Lambda\bar\partial-\bar\partial\Lambda\partial-\partial\bar\partial\Lambda-\Lambda\partial\bar\partial\right)\\
&=\Delta_{\bar\partial}.
\end{aligned}
$$

Finally expand $d=\partial+\bar\partial$ and $d^*=\partial^*+\bar\partial^*$; the mixed terms just proved zero disappear. This derives the [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md)

$$
\boxed{\Delta_d=\Delta_\partial+\Delta_{\bar\partial}=2\Delta_{\bar\partial}.}
$$

The [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) preserves bidegree. Thus the complex $d$-harmonic forms of total degree $r$ split into their harmonic $(p,q)$ parts. The allowed real [Hodge theorem](../../../../../hodge-decomposition-theorem.md), followed by complexification, gives

$$
b^r(X)=\sum_{p+q=r}h^{p,q},\qquad h^{p,q}=\dim_{\mathbb C}\mathcal H_{\bar\partial}^{p,q}.
$$

The real operator $\Delta_d$ commutes with conjugation, which exchanges $(p,q)$ and $(q,p)$. Therefore $h^{p,q}=h^{q,p}$. For odd $r$, no summand has $p=q$, so they pair off in equal dimensions. This proves that **all odd Betti numbers are even**.

For $1\leq k\leq n$, the [Kähler form](../../../../../kahler-form.md) power $\omega^k$ is closed. If it were exact, say $\omega^k=d\eta$, then

$$
\int_X\omega^n=\int_Xd(\eta\wedge\omega^{n-k})=0
$$

by [Stokes theorem](../../../../../stokes-theorem.md). But $\omega^n=n!\operatorname{vol}_g$ has strictly positive integral on the nonempty compact manifold. Hence the [powers of a compact Kähler form have nonzero cohomology classes](../../../../../powers-of-a-compact-kahler-form-have-nonzero-cohomology-classes.md), and

$$
\boxed{b^{2k-1}(X)\in2\mathbb Z_{\geq0},\qquad b^{2k}(X)\geq1\quad(1\leq k\leq n).}
$$

For an example take the [Hopf surface](../../../../../hopf-surface.md)

$$
H=(\mathbb C^2\setminus\{0\})/\langle z\mapsto2z\rangle.
$$

The dilation action is free and properly discontinuous: on a compact subset the radii are bounded above and away from zero, so only finitely many dilations can meet it. It is holomorphic, giving a [complex manifold](../../../../../complex-manifold.md) quotient; the annulus $1\leq\|z\|\leq2$ covers the quotient, proving compactness. The map

$$
[z]\longmapsto\left(z/\|z\|,\ \log\|z\|\bmod\log2\right)
$$

is a [diffeomorphism](../../../../../diffeomorphism.md) $H\cong S^3\times S^1$. The [Künneth theorem](../../../../../kunneth-theorem.md) gives $b^1(H)=1$. This violates the necessary odd-degree parity, so **this compact complex surface admits no Kähler metric**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
