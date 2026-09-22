<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [real (1, 1)-form](../../../../../real-1-1-form.md) is a form $\varphi\in\Omega^{1,1}(X)$ satisfying $\bar\varphi=\varphi$. In holomorphic coordinates it has the form

$$
\varphi=i\sum_{j,k}h_{j\bar k}\,dz^j\wedge d\bar z^k,
\qquad h_{j\bar k}=\overline{h_{k\bar j}}.
$$

It is a [positive real (1, 1)-form](../../../../../positive-real-1-1-form.md) when

$$
-i\varphi(\xi,\bar\xi)>0
$$

for every nonzero tangent vector $\xi$ of type $(1,0)$, equivalently when the [Hermitian matrix](../../../../../hermitian-operator.md) $(h_{j\bar k})$ is positive definite.

A [holomorphic local trivialization](../../../../../holomorphic-local-trivialization.md) of a [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) $L\to X$ is equivalently a nowhere-zero [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) $e$. A connection $A$ is [unitary](../../../../../unitary-connection.md) when it preserves the fiberwise Hermitian inner product:

$$
d\,h(s,t)=h(\nabla^As,t)+h(s,\nabla^At).
$$

The [Chern connection](../../../../../chern-connection.md) is the unique unitary connection whose $(0,1)$ part is the bundle's [Dolbeault partial connection](../../../../../dolbeault-partial-connection.md) $\bar\partial_L$.

In a holomorphic frame, put $h=h(e,e)$. The [local formula for the Chern connection on a line bundle](../../../../../local-formula-for-the-chern-connection-on-a-line-bundle.md) is

$$
\nabla^Ae=(\partial\log h)e,
\qquad
F(A)=\bar\partial\partial\log h.
$$

The curvature therefore has type $(1,1)$. Since a unitary connection has imaginary curvature, $\overline{F(A)}=-F(A)$, and hence

$$
\overline{iF(A)}=iF(A).
$$

Thus $iF(A)$ is a real $(1,1)$-form.

For connections $A$ on $L$ and $\widehat A$ on $\widehat L$, the [tensor product connection](../../../../../tensor-product-connection.md) is defined on decomposable local sections by

$$
\nabla^{A\otimes\widehat A}(s\otimes\widehat s)
=\nabla^As\otimes\widehat s+s\otimes\nabla^{\widehat A}\widehat s.
$$

The [curvature of a tensor product connection](../../../../../curvature-of-a-tensor-product-connection.md) on line bundles is additive:

$$
F(A\otimes\widehat A)=F(A)+F(\widehat A).
$$

Consequently

$$
iF(A\otimes\widehat A)=iF(A)+iF(\widehat A),
$$

which is positive whenever both summands are positive.

For the final assertion, simultaneously diagonalize the positive Hermitian matrices of $\varphi$ and $\psi$ by congruence at the chosen point. In the resulting coframe,

$$
\varphi=i\sum_ja_jdz^j\wedge d\bar z^j,
\qquad
\psi=i\sum_jb_jdz^j\wedge d\bar z^j,
\qquad a_j,b_j>0.
$$

A direct wedge-product calculation gives

$$
(\varphi\wedge\psi)(\xi,\eta,\bar\xi,\bar\eta)
=\sum_{j<k}(a_jb_k+a_kb_j)
|\xi_j\eta_k-\xi_k\eta_j|^2.
$$

If $\xi$ and $\eta$ are linearly independent, at least one of these $2\times2$ minors is nonzero. Every coefficient is positive, so the sum is strictly positive. This is [wedge positivity for two positive (1, 1)-forms](../../../../../wedge-positivity-for-two-positive-1-1-forms.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
