<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Riemannian volume form](../../../../../riemannian-volume-form.md) of an oriented $n$-dimensional [Riemannian manifold](../../../../../riemannian-manifold.md) is the unique positive $n$-form taking value one on every positively oriented orthonormal frame. In positive coordinates,

$$
\omega_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

The metric induces an inner product on exterior powers of the [cotangent bundle](../../../../../cotangent-bundle.md), with wedges of distinct orthonormal covectors forming an [orthonormal basis](../../../../../orthonormal-basis.md). The [Hodge star](../../../../../hodge-star-operator.md) is the pointwise linear map $*:\Lambda^pT^*M\to\Lambda^{n-p}T^*M$ specified by

$$
\alpha\wedge*\beta=\langle\alpha,\beta\rangle_g\omega_g.
$$

It is an [isometry](../../../../../isometry.md) and satisfies $**\alpha=(-1)^{p(n-p)}\alpha$. With the positive-sign convention, the [Hodge Laplacian](../../../../../hodge-laplacian.md) on [differential forms](../../../../../differential-form-split.md) is

$$
\Delta=d\delta+\delta d,\qquad
\delta|_{\Omega^p}=(-1)^{n(p-1)+1}*d*.
$$

Here $d$ is the [exterior derivative](../../../../../exterior-derivative.md) and $\delta$ its [formal adjoint](../../../../../formal-adjoint.md); $\delta$ on functions is zero. On functions this is the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md)

$$
\Delta f=-\operatorname{div}(\operatorname{grad}f)
=-\frac1{\sqrt{\det g}}\partial_i\bigl(\sqrt{\det g}\,g^{ij}\partial_jf\bigr).
$$

The convention $\operatorname{div}\operatorname{grad}$ gives the negative of this operator. All subsequent Laplacians use the nonnegative convention above.

On a compact oriented manifold without boundary, the [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) gives an orthogonal decomposition of smooth real forms,

$$
\Omega^p(M)=\mathcal H^p(M)\oplus d\Omega^{p-1}(M)\oplus\delta\Omega^{p+1}(M),\qquad
\mathcal H^p=\ker\Delta.
$$

The three component forms are uniquely determined, although the potentials in the last two summands need not be unique. The space $\mathcal H^p$ is finite-dimensional, and each [de Rham cohomology](../../../../../de-rham-cohomology.md) class has a unique harmonic representative. [Integration by parts](../../../../../integration-by-parts.md) gives $\langle\Delta\alpha,\alpha\rangle_{L^2}=\|d\alpha\|_{L^2}^2+\|\delta\alpha\|_{L^2}^2$, so [harmonic forms](../../../../../harmonic-differential-form.md) are exactly the closed and coclosed forms. Set $\Omega^k=0$ outside $0\le k\le n$. Compactness without boundary is a hypothesis of this version of the theorem; orientation alone does not supply it.

A connection on $TM$ induces a [dual connection](../../../../../dual-connection.md) on $T^*M$ and then connections on its tensor and exterior powers by the Leibniz rule. Explicitly, for a $p$-form $\alpha$,

$$
(\nabla_X\alpha)(Y_1,\ldots,Y_p)=X\bigl(\alpha(Y_1,\ldots,Y_p)\bigr)
-\sum_{j=1}^p\alpha(Y_1,\ldots,\nabla_XY_j,\ldots,Y_p).
$$

To prove the [parallelism of the Riemannian volume form](../../../../../parallelism-of-the-riemannian-volume-form.md), use a local positively oriented orthonormal frame $E_i$, its dual coframe $\theta^i$, and write $\nabla_XE_j=\sum_i a_{ij}(X)E_i$. [Metric compatibility](../../../../../metric-compatibility.md) makes the matrix $a(X)$ skew-symmetric. Since $\omega_g=\theta^1\wedge\cdots\wedge\theta^n$, differentiating the wedge yields

$$
\nabla_X\omega_g=-\sum_i a_{ii}(X)\omega_g=0.
$$

Off-diagonal terms vanish because they repeat a coframe factor. Thus **$\nabla\omega_g=0$**; equivalently [parallel transport](../../../../../parallel-transport.md) preserves both the metric and the continuously chosen orientation.

Now let $M$ be compact, oriented and without boundary. For [representing functionals on harmonic forms by wedge pairing](../../../../../representing-functionals-on-harmonic-forms-by-wedge-pairing.md), choose an $L^2$-[orthonormal basis](../../../../../orthonormal-basis.md) $h_1,\ldots,h_b$ of $\mathcal H^p$ and define

$$
h_f=\sum_{a=1}^b f(h_a)h_a,\qquad \psi_0=*h_f.
$$

If $\varphi=\sum_a c_ah_a$, linearity gives

$$
\boxed{f(\varphi)=\langle\varphi,h_f\rangle_{L^2}=\int_M\varphi\wedge\psi_0}.
$$

This also works when $b=0$, using the empty sum. Since the [Hodge star](../../../../../hodge-star-operator.md) commutes with the [Hodge Laplacian](../../../../../hodge-laplacian.md), $\psi_0$ is harmonic of degree $n-p$.

For the full [ambiguity of harmonic wedge-pairing representatives](../../../../../ambiguity-of-harmonic-wedge-pairing-representatives.md), write another representative as $\psi_0+\chi$. Because the star is an [isometry](../../../../../isometry.md),

$$
\int_M\varphi\wedge\chi=\langle*\varphi,\chi\rangle_{L^2}.
$$

The forms $*\varphi$ range over all of $\mathcal H^{n-p}$. Hence $\chi$ gives zero functional exactly when its harmonic projection is zero. Hodge decomposition proves that the complete answer is

$$
\boxed{\psi=*h_f+d\alpha+\delta\beta,\qquad
\alpha\in\Omega^{n-p-1}(M),\quad\beta\in\Omega^{n-p+1}(M)}.
$$

Both summands in this ambiguity are permitted; it is not only an exact-form ambiguity. The exact and coexact component forms are orthogonal to every [harmonic form](../../../../../harmonic-differential-form.md), so every displayed choice works. Conversely a nonzero harmonic component would pair nontrivially with some $*\varphi$, and therefore cannot occur. **The harmonic representative $*h_f$ is unique; the arbitrary smooth representative generally is not.** The formula also covers the endpoint degrees and any exceptional case where the ambiguity space is zero.

For a concrete coexact ambiguity, take the [torus](../../../../../torus.md) $(\mathbb R/2\pi\mathbb Z)^2$ with metric $dx^2+dy^2$. The form $\chi=\delta(\sin y\,dx\wedge dy)=\cos y\,dx$ annihilates every harmonic one-form by orthogonality, yet $d\chi=\sin y\,dx\wedge dy$ is nonzero. Thus an annihilating representative need not even be closed, let alone exact.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
