<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Kähler manifold](../../../../../kahler-manifold.md) structure gives a [Riemannian metric](../../../../../riemannian-metric.md), its volume form, the complex orientation, and a Hermitian inner product on complex differential forms. The [complex Hodge star operator](../../../../../complex-hodge-star-operator.md) is the complex-linear map characterized by

$$
\alpha\wedge *\bar\beta
=\langle\alpha,\beta\rangle\operatorname{vol}_g.
$$

On $r$-forms in real dimension $m=2n$, the [codifferential](../../../../../codifferential.md) is

$$
d^*=(-1)^{m(r+1)+1}*d*,
$$

equivalently the [formal adjoint](../../../../../formal-adjoint.md) of $d$ for the $L^2$ inner product. Similarly $\bar\partial^*$ is the formal adjoint of $\bar\partial$. Define the [Hodge Laplacian](../../../../../hodge-laplacian.md) and [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) by

$$
\Delta_d=dd^*+d^*d,
\qquad
\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.
$$

Expanding $d=\partial+\bar\partial$, the [Kähler identities](../../../../../kahler-identities.md) make the mixed anticommutators vanish and imply $\Delta_\partial=\Delta_{\bar\partial}$. Hence the [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md) is

$$
\Delta_d=2\Delta_{\bar\partial}.
$$

Let $L\gamma=\omega\wedge\gamma$ be the [Lefschetz operator of a Kähler manifold](../../../../../lefschetz-operator-of-a-kahler-manifold.md). The Kähler identities also imply

$$
[L,\Delta_{\bar\partial}]=0.
$$

Thus, if $\Delta_{\bar\partial}\alpha=0$, then

$$
\Delta_{\bar\partial}(\alpha\wedge\omega^k)
=\Delta_{\bar\partial}L^k\alpha
=L^k\Delta_{\bar\partial}\alpha=0.
$$

This is the fact that the [Lefschetz operator preserves harmonic forms](../../../../../lefschetz-operator-preserves-harmonic-forms.md).

The [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) states that

$$
\Omega^{p,q}(X)
=\mathcal H_{\bar\partial}^{p,q}
\oplus\bar\partial\Omega^{p,q-1}(X)
\oplus\bar\partial^*\Omega^{p,q+1}(X),
$$

an orthogonal direct sum, where $\mathcal H_{\bar\partial}^{p,q}=\ker\Delta_{\bar\partial}$.

Suppose $\eta=\bar\partial\gamma$ has type $(p,q)$. Apply this decomposition to $\gamma\in\Omega^{p,q-1}$. The harmonic and $\bar\partial$-exact pieces disappear after applying $\bar\partial$, so for some $\beta\in\Omega^{p,q}$,

$$
\eta=\bar\partial\bar\partial^*\beta.
$$

Put $\theta=\bar\partial^*\beta$. If also $\partial\eta=0$, then

$$
\bar\partial(\partial\theta)=-\partial(\bar\partial\theta)=-\partial\eta=0.
$$

The Kähler anticommutation identity $\bar\partial^*\partial+\partial\bar\partial^*=0$ and $(\bar\partial^*)^2=0$ give

$$
\bar\partial^*(\partial\theta)
=-\partial(\bar\partial^*\theta)=0.
$$

Therefore $\partial\theta$ is $\Delta_{\bar\partial}$-harmonic. By $\Delta_\partial=\Delta_{\bar\partial}$ it is also $\partial$-harmonic, but it is $\partial$-exact; orthogonality of harmonic and exact forms forces

$$
\partial\theta=0.
$$

This proves both requested claims: $\partial\bar\partial^*\beta=0$ is harmonic, and $\bar\partial^*\beta=\theta$ is $\partial$-closed.

Finally, $\theta\in\operatorname{im}\bar\partial^*$ is orthogonal to $\ker\bar\partial$, and hence to every $\bar\partial$-harmonic form. Since the $\partial$- and $\bar\partial$-harmonic spaces agree on a compact Kähler manifold, the $\partial$-closed form $\theta$ has zero harmonic component in its $\partial$-Hodge decomposition. It follows that $\theta=\partial\phi$ for some $\phi\in\Omega^{p-1,q-1}(X)$. Hence

$$
\eta=\bar\partial\theta=\bar\partial\partial\phi,
$$

which is the [ddbar lemma](../../../../../ddbar-lemma.md) in this case.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
