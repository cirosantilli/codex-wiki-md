<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $g$ be the real [Riemannian metric](../../../../../riemannian-metric.md) underlying the [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md), and let $J$ be the [complex structure](../../../../../complex-structure.md). The [fundamental form of a Hermitian manifold](../../../../../fundamental-form-of-a-hermitian-manifold.md) is

$$
\omega(u,v)=g(Ju,v).
$$

The identity $g(Ju,Jv)=g(u,v)$ implies $g(Ju,v)=-g(u,Jv)$, so this is an alternating real two-form. Moreover $\omega(Ju,Jv)=\omega(u,v)$. A two-form with this invariance has type $(1,1)$: on two vectors of type $(1,0)$, applying $J$ to both multiplies its value by $i^2=-1$, forcing that value to vanish; the same argument applies to type $(0,1)$. Hence **$\omega$ is a real $(1,1)$-form**.

Use the complex-linear convention for the [complex Hodge star operator](../../../../../complex-hodge-star-operator.md), extending the real star. The complex orientation and metric define $dV=\omega^n/n!$, and

$$
\alpha\wedge *\bar\beta=\langle\alpha,\beta\rangle_g\,dV,
\qquad *:\mathcal A^{p,q}\longrightarrow\mathcal A^{n-q,n-p},
\qquad *^2=(-1)^{r(2n-r)}\ \text{on total degree }r.
$$

Here the [Hermitian inner product](../../../../../hermitian-form.md) is linear in the first argument. With this convention, on the even-dimensional underlying real manifold the [formal adjoints](../../../../../formal-adjoint.md) are $d^*=-*d*$, $\bar\partial^*=-*\partial*$ and $\partial^*=-*\bar\partial*$. A conjugate-linear star is another convention, but then the adjoint formulas must change accordingly.

The [Hodge Laplacian](../../../../../hodge-laplacian.md) and [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) are

$$
\Delta_d=dd^*+d^*d,\qquad
\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.
$$

Also write $\Delta_\partial=\partial\partial^*+\partial^*\partial$. They are nonnegative, since for example

$$
(\Delta_{\bar\partial}\alpha,\alpha)_{L^2}
=\|\bar\partial\alpha\|_{L^2}^2+\|\bar\partial^*\alpha\|_{L^2}^2.
$$

The requested [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) is a [compactness](../../../../../compact-space.md) statement: on a [compact](../../../../../compact-space.md) Hermitian manifold without boundary,

$$
\mathcal A^{p,q}=\mathcal H^{p,q}_{\bar\partial}
\mathbin{\oplus^{\perp}}\bar\partial\mathcal A^{p,q-1}
\mathbin{\oplus^{\perp}}\bar\partial^*\mathcal A^{p,q+1},
\qquad \mathcal H^{p,q}_{\bar\partial}=\ker\Delta_{\bar\partial}.
$$

The harmonic space is finite-dimensional, and taking the harmonic representative induces an isomorphism $\mathcal H^{p,q}_{\bar\partial}\cong H^{p,q}_{\bar\partial}(X)$. [Compactness](../../../../../compact-space.md) is essential to this formulation; it is not asserted on an arbitrary noncompact Hermitian manifold.

Now suppose $X$ is [compact](../../../../../compact-space.md) and [Kähler](../../../../../kahler-manifold.md), so $d\omega=0$. The permitted [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md) is $\Delta_d=2\Delta_{\bar\partial}=2\Delta_\partial$, making the three harmonic spaces identical in each bidegree. A $d$-closed pure-type form has $\partial\alpha=\bar\partial\alpha=0$, since these two terms have different types. We will construct a [Green operator potential for ddbar exactness](../../../../../green-operator-potential-for-ddbar-exactness.md), rather than invoking the [ddbar lemma](../../../../../ddbar-lemma.md) as the conclusion to be proved.

Let $G$ be the inverse of $\Delta_{\bar\partial}$ on the [orthogonal complement](../../../../../orthogonal-complement.md) of its [harmonic forms](../../../../../harmonic-differential-form.md), zero on the harmonic space. It is twice the [Green operator of the Hodge Laplacian](../../../../../green-operator-of-the-hodge-laplacian.md). The [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) and elliptic inversion give $\Delta_{\bar\partial}G=I-H$, with $H$ harmonic projection. It preserves bidegrees. The operators $\partial$ and $\bar\partial$ commute with $\Delta_{\bar\partial}$: the first follows from $\Delta_{\bar\partial}=\Delta_\partial$ and $\partial^2=0$, and the second directly from $\bar\partial^2=0$. They and their [formal adjoints](../../../../../formal-adjoint.md) annihilate [harmonic forms](../../../../../harmonic-differential-form.md), so they preserve the [orthogonal complement](../../../../../orthogonal-complement.md) of the harmonic space. Consequently they commute with $G$, by uniqueness of the inverse on the harmonic complement. Thus $u=G\alpha$ and $v=G^2\alpha$ are killed by both differential operators.

The assumed orthogonality makes $H\alpha=Hu=0$. Applying the two Laplacians gives

$$
\alpha=\Delta_{\bar\partial}u=\bar\partial\bar\partial^*u,
\qquad u=\Delta_\partial v=\partial\partial^*v.
$$

We also need the mixed anticommutator, which follows from the permitted Laplacian identity rather than an extra unproved lemma. Expand $\Delta_d$ using $d=\partial+\bar\partial$ and $d^*=\partial^*+\bar\partial^*$. Since $\Delta_d=\Delta_\partial+\Delta_{\bar\partial}$, its mixed terms sum to zero. Their two bidegrees $(1,-1)$ and $(-1,1)$ are distinct, so each vanishes separately, in particular $\bar\partial^*\partial+\partial\bar\partial^*=0$. Hence

$$
\alpha=\bar\partial\bar\partial^*\partial\partial^*v
=-\bar\partial\partial\bar\partial^*\partial^*v
=\partial\bar\partial\bigl(\bar\partial^*\partial^*v\bigr).
$$

We have obtained the explicit answer

$$
\boxed{\alpha=\partial\bar\partial\beta,\qquad
\beta=\bar\partial^*\partial^*G^2\alpha\in\mathcal A^{p-1,q-1}.}
$$

The positive assumptions on $p,q$ ensure these degrees are available. Conversely such a form is orthogonal to [harmonic forms](../../../../../harmonic-differential-form.md) by integration by parts, so the same proof also explains the [harmonic orthogonality criterion for ddbar exactness](../../../../../harmonic-orthogonality-criterion-for-ddbar-exactness.md).

For injectivity of the [Lefschetz operator on a Hermitian manifold](../../../../../lefschetz-operator-on-a-hermitian-manifold.md) on real one-forms, work at one point in a metric-orthonormal coframe $(e^1,f^1,\ldots,e^n,f^n)$ with $\omega=\sum_j e^j\wedge f^j$. If $a\ne0$, a unitary change of coframe makes $a=ce^1$, $c\ne0$. Then

$$
a\wedge\omega=c\sum_{j=2}^n e^1\wedge e^j\wedge f^j\ne0\quad(n>1),
$$

since the displayed basis three-forms are linearly independent. Therefore $L(a)=a\wedge\omega$ has zero kernel. Injectivity on complex one-forms follows by taking real and imaginary parts, since $\omega$ is real. This pointwise proof of [injectivity of powers of the Lefschetz operator](../../../../../injectivity-of-powers-of-the-lefschetz-operator.md) for degree one does not require the hard Lefschetz theorem.

Closedness of $\omega$ gives $\bar\partial L=L\bar\partial$. Using the permitted [Kähler identities](../../../../../kahler-identities.md), specifically $[\bar\partial^*,L]=i\partial$, gives

$$
[\Delta_{\bar\partial},L]
=\bar\partial[\bar\partial^*,L]+[\bar\partial^*,L]\bar\partial
=i(\bar\partial\partial+\partial\bar\partial)=0.
$$

Multiplying by two proves **$[\Delta_d,L]=0$**. In particular the [Lefschetz operator preserves harmonic forms](../../../../../lefschetz-operator-preserves-harmonic-forms.md) and the injective map on one-forms restricts to an injection $\mathcal H_d^1\hookrightarrow\mathcal H_d^3$. The de Rham [Hodge theorem](../../../../../hodge-decomposition-theorem.md) identifies these real harmonic spaces with the corresponding real cohomology groups. Taking dimensions yields

$$
\boxed{b^3(X)\ge b^1(X).}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
