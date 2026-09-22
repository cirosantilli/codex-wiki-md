<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $g=\operatorname{Re}h$ for the underlying [Riemannian metric](../../../../../riemannian-metric.md) of the [Hermitian manifold](../../../../../hermitian-manifold.md). Its [fundamental form of a Hermitian manifold](../../../../../fundamental-form-of-a-hermitian-manifold.md) is

$$
\omega(u,v)=g(Ju,v).
$$

It is real and skew-symmetric. In a unitary coframe it is $\omega=\sum_{j=1}^n e^j\wedge Je^j$, which also shows that it has type $(1,1)$ and that

$$
\operatorname{vol}_g=\frac{\omega^n}{n!}.
$$

The [Hodge star operator](../../../../../hodge-star-operator.md) is characterized, after complex-linear extension, by

$$
\alpha\wedge *\overline\beta=\langle\alpha,\beta\rangle\operatorname{vol}_g.
$$

Expanding in the same unitary coframe gives

$$
*\omega=\frac{\omega^{n-1}}{(n-1)!}.
$$

The [Hodge Laplacian](../../../../../hodge-laplacian.md) and [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) are

$$
\Delta_d=dd^*+d^*d,
\qquad
\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.
$$

The [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) says that every Dolbeault class has a unique $\Delta_{\bar\partial}$-harmonic representative and

$$
\Omega^{p,q}=\mathcal H^{p,q}_{\bar\partial}\oplus\bar\partial\Omega^{p,q-1}\oplus\bar\partial^*\Omega^{p,q+1}.
$$

If $\Delta_{\bar\partial}\eta=0$, then

$$
0=\langle\Delta_{\bar\partial}\eta,\eta\rangle
=\|\bar\partial\eta\|_2^2+\|\bar\partial^*\eta\|_2^2,
$$

so $\eta$ is $\bar\partial$-closed and $\bar\partial^*$-closed. If also $\eta=\bar\partial\xi$, then $\|\eta\|_2^2=\langle\bar\partial^*\eta,\xi\rangle=0$, hence $\eta=0$.

Now suppose $X$ is compact and [Kähler](../../../../../kahler-manifold.md). With $d^c=i(\bar\partial-\partial)$ and $d^*=\partial^*+\bar\partial^*$, the [Kähler identities](../../../../../kahler-identities.md) make the mixed anticommutators vanish and give $\Delta_\partial=\Delta_{\bar\partial}$. Consequently

$$
d^cd^*+d^*d^c=0.
$$

Let $\alpha=d^c\gamma$ and $d\alpha=0$. The [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md) implies that the $d$-Laplacian commutes with $d^c$. Since a harmonic form is $d^{c*}$-closed, $\alpha$ is orthogonal to every harmonic form. If $G$ is the [Green operator of the Hodge Laplacian](../../../../../green-operator-of-the-hodge-laplacian.md), then

$$
\alpha=\Delta_dG\alpha=dd^*G\alpha,
$$

where the $d^*dG\alpha$ term vanishes because $dG\alpha=Gd\alpha=0$. The Green operator commutes with $d^c$, and the anticommutation identity just proved gives

$$
d^*G\alpha=d^*d^cG\gamma=-d^cd^*G\gamma.
$$

Therefore, for the $(k-2)$-form $\beta=-d^*G\gamma$,

$$
\boxed{\alpha=dd^c\beta.}
$$

This is the [d d c lemma](../../../../../ddc-lemma.md) in the form required here.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
