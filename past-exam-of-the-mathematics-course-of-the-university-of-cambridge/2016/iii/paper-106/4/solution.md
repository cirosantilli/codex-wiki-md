<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The definitions in a unital [C-star algebra](../../../../../c-star-algebra.md) are

$$
\boxed{\begin{array}{ll}
\text{hermitian:}&x^*=x,\\
\text{unitary:}&x^*x=xx^*=1,\\
\text{normal:}&x^*x=xx^*.
\end{array}}
$$

Thus a [Hermitian element of a C-star algebra](../../../../../hermitian-element-of-a-c-star-algebra.md) is self-adjoint, a [Unitary element of a C-star algebra](../../../../../unitary-element-of-a-c-star-algebra.md) has inverse $x^*$, and a [Normal element of a C-star algebra](../../../../../normal-element-of-a-c-star-algebra.md) commutes with its adjoint. We derive the needed [C-star algebra](../../../../../c-star-algebra.md) facts directly from $\|a^*a\|=\|a\|^2$, as required.

First $\|1\|=\|1\|^2$ gives $\|1\|=1$, and

$$
\|a\|^2=\|a^*a\|\le\|a^*\|\|a\|
$$

gives $\|a\|\le\|a^*\|$; applying the same argument to $a^*$ gives equality. Thus the involution is an [isometry](../../../../../isometry.md). For a [Unitary element of a C-star algebra](../../../../../unitary-element-of-a-c-star-algebra.md) $u$,

$$
\|u\|^2=\|u^*u\|=1,\qquad\|u^{-1}\|=\|u^*\|=1.
$$

The general [Banach algebra](../../../../../banach-algebra-split.md) [spectrum](../../../../../spectrum-functional-analysis.md) bound gives $|\lambda|\le1$ for $\lambda\in\sigma(u)$. Such a $\lambda$ is nonzero, and the inverse [spectral mapping theorem](../../../../../spectral-mapping-theorem.md) gives $\lambda^{-1}\in\sigma(u^{-1})$, so also $|\lambda|^{-1}\le1$. Hence

$$
\boxed{\sigma(u)\subseteq\mathbb T=\{z\in\mathbb C:|z|=1\}.}
$$

If $h=h^*$, the convergent [exponential series](../../../../../exponential-series.md) and the isometric involution give $(e^{ith})^*=e^{-ith}$. These commuting exponentials multiply to $1$, so $e^{ith}$ is unitary for real $t$. By the exponential [spectral mapping theorem](../../../../../spectral-mapping-theorem.md), if $\lambda\in\sigma(h)$ then $e^{it\lambda}\in\sigma(e^{ith})\subseteq\mathbb T$. Taking $t=1$ gives $e^{-\operatorname{Im}\lambda}=1$, so

$$
\boxed{\sigma(h)\subseteq\mathbb R.}
$$

Only general [Banach algebra](../../../../../banach-algebra-split.md) [spectral mapping theorem](../../../../../spectral-mapping-theorem.md) and the defining [C-star identity](../../../../../c-star-identity.md) were used.

Now prove [spectral permanence for C-star algebras](../../../../../spectral-permanence-for-c-star-algebras.md). Let $B\subseteq A$ be the norm-closed [C-star subalgebra](../../../../../c-star-subalgebra.md) with the same identity. The algebraic inclusion always gives $\sigma_A(b)\subseteq\sigma_B(b)$. For $h=h^*\in B$, both [spectra](../../../../../spectrum-functional-analysis.md) lie in $\mathbb R$. If $\lambda\notin\sigma_A(h)$, choose nonreal $\lambda_n\to\lambda$. Since $\sigma_B(h)\subseteq\mathbb R$, each $(\lambda_n1-h)^{-1}$ belongs to $B$. By [continuity of inversion in a Banach algebra](../../../../../continuity-of-inversion-in-a-banach-algebra.md), these inverses converge in $A$ to $(\lambda1-h)^{-1}$, which belongs to $B$ because $B$ is closed. Thus $\lambda\notin\sigma_B(h)$, proving equality for hermitian elements.

For the requested normal $x\in B$, suppose $b=x-\lambda1$ is invertible in $A$. The element $b^*b$ is hermitian and invertible in $A$, so the equality just proved places $(b^*b)^{-1}$ in $B$. Consequently

$$
y=(b^*b)^{-1}b^*\in B,\qquad yb=1.
$$

Since $b$ already has a two-sided inverse in $A$, multiplying $yb=1$ by that inverse gives $y=b^{-1}$. Hence its inverse belongs to $B$, and

$$
\boxed{\sigma_B(x)=\sigma_A(x).}
$$

We need one more elementary consequence of the [C-star identity](../../../../../c-star-identity.md): the [spectral radius norm equality for normal elements](../../../../../spectral-radius-norm-equality-for-normal-elements.md). If $h=h^*$, then $\|h^2\|=\|h\|^2$. If $a$ is normal, commutativity of $a,a^*$ gives

$$
\|a^2\|^2=\|(a^*)^2a^2\|=\|(a^*a)^2\|=\|a^*a\|^2=\|a\|^4.
$$

Every power of $a$ is a [Normal element of a C-star algebra](../../../../../normal-element-of-a-c-star-algebra.md). Induction gives $\|a^{2^n}\|=\|a\|^{2^n}$. The general [spectral radius formula](../../../../../spectral-radius-formula.md) therefore implies

$$
r(a)=\lim_{m\to\infty}\|a^m\|^{1/m}=\|a\|.
$$

**The continuous functional calculus is the unique unital $*$-homomorphism $C(K)\to\mathcal B(H)$ taking the coordinate function to $T$.** For [bounded linear operators](../../../../../continuous-linear-operator.md) on a [Hilbert space](../../../../../hilbert-space-split.md), the adjoint identity gives $\|S\|=\sup_{\|v\|=\|w\|=1}|\langle Sv,w\rangle|=\|S^*\|$. Therefore

$$
\|S\|^2=\sup_{\|v\|=1}\langle S^*Sv,v\rangle\le\|S^*S\|\le\|S^*\|\|S\|=\|S\|^2.
$$

This proves the [C-star identity](../../../../../c-star-identity.md) for $\mathcal B(H)$ directly; completeness and submultiplicativity come from the operator norm. Let

$$
C=\overline{\{p(T,T^*):p\text{ a complex polynomial in two commuting variables}\}}^{\,\|\cdot\|}.
$$

Because $T$ is a [normal operator](../../../../../normal-operator.md), this is a commutative unital [C-star algebra](../../../../../c-star-algebra.md). Every element of $C$ is a [Normal element of a C-star algebra](../../../../../normal-element-of-a-c-star-algebra.md), so the preceding norm identity says its [Gelfand transform](../../../../../gelfand-representation.md) is isometric:

$$
\|\widehat a\|_\infty=\sup_{\chi\in\Delta(C)}|\chi(a)|=r_C(a)=\|a\|.
$$

Here $\Delta(C)$ is the compact [character space](../../../../../character-space-of-an-algebra.md) from the general [Gelfand representation theorem](../../../../../gelfand-representation-theorem.md) for commutative [Banach algebras](../../../../../banach-algebra-split.md).

Each [algebra character](../../../../../character-of-an-algebra.md) preserves the involution. Indeed, write $a=h+ik$ with $h,k$ hermitian; $\chi(h)\in\sigma_C(h)\subseteq\mathbb R$ and similarly for $k$, so $\chi(a^*)=\overline{\chi(a)}$. Therefore the continuous map

$$
\Delta(C)\longrightarrow K,\qquad\chi\longmapsto\chi(T)
$$

is injective: its value determines $\chi(T^*)$ and hence its value on all the dense [polynomials](../../../../../polynomial-split.md). It is surjective because the general character description of the [spectrum](../../../../../spectrum-functional-analysis.md) gives $\{\chi(T):\chi\in\Delta(C)\}=\sigma_C(T)$, and [spectral permanence for C-star algebras](../../../../../spectral-permanence-for-c-star-algebras.md) identifies this with $\sigma_{\mathcal B(H)}(T)=K$. A [continuous function](../../../../../continuous-function.md) that is a bijection from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md), so we identify $\Delta(C)$ with $K$.

Under this identification, the [Gelfand transform](../../../../../gelfand-representation.md) sends $T$ to $u(z)=z$ and $T^*$ to $\overline u$. Its image is an isometric, and therefore closed, unital self-adjoint subalgebra of $C(K)$. It separates points because it contains $u$. The complex [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes the image dense, hence equal to all of $C(K)$. Inverting the [Gelfand transform](../../../../../gelfand-representation.md) and including $C$ into $\mathcal B(H)$ gives

$$
\Phi:C(K)\longrightarrow\mathcal B(H),\qquad f\longmapsto f(T),
$$

an isometric unital [C-star homomorphism](../../../../../c-star-homomorphism.md) with $u(T)=T$.

To prove uniqueness without assuming automatic continuity of [C-star homomorphisms](../../../../../c-star-homomorphism.md), let $\Psi$ be any other such map. Since every $f\in C(K)$ is normal, $\Psi(f)$ is normal. A unital algebra homomorphism preserves inverses, so

$$
\sigma_{\mathcal B(H)}(\Psi(f))\subseteq\sigma_{C(K)}(f)=f(K).
$$

Using the normal-element norm identity yields $\|\Psi(f)\|=r(\Psi(f))\le\|f\|_\infty$. Thus $\Psi$ is contractive. It agrees with $\Phi$ on [polynomials](../../../../../polynomial-split.md) in $u,\overline u$, since both send them to the same [polynomials](../../../../../polynomial-split.md) in $T,T^*$. These [polynomials](../../../../../polynomial-split.md) are dense by the [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md), so continuity proves $\Psi=\Phi$. This establishes the [continuous functional calculus](../../../../../continuous-functional-calculus.md) with no unproved theorem specific to [C-star algebras](../../../../../c-star-algebra.md).

**A disconnected spectrum gives a nontrivial closed invariant subspace.** Write $K=K_1\sqcup K_2$ with $K_1,K_2$ nonempty and both open and closed in $K$. The [indicator function](../../../../../indicator-function.md) $f=\mathbf1_{K_1}$ is continuous on $K$, even though no such continuity is needed across the gap outside $K$. Let $P=f(T)$. The [continuous functional calculus](../../../../../continuous-functional-calculus.md) gives

$$
P^2=P,\qquad P^*=P,\qquad PT=TP.
$$

Its isometry gives $\|P\|=1$ and $\|I-P\|=1$, so $P\ne0,I$. The [linear projection](../../../../../projection-linear-algebra.md) has closed range $Y=PH=\ker(I-P)$. Its range is nonzero and proper, and $T(Px)=P(Tx)\in Y$ proves invariance. Since it also commutes with $T^*$, the same subspace is reducing. This proves [disconnected spectrum gives a reducing subspace](../../../../../disconnected-spectrum-gives-a-reducing-subspace.md).

<a id="4/image-a-disconnected-spectrum-and-its-continuous-indicator-which-produces-a-nontrivial-reducing-projection"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106-disconnected-spectrum.png)

**[Figure 1](#4/image-a-disconnected-spectrum-and-its-continuous-indicator-which-produces-a-nontrivial-reducing-projection). A disconnected spectrum and its continuous indicator, which produces a nontrivial reducing projection**.

The figure can be realized without any [eigenvalues](../../../../../eigenvalue.md): take $H=L^2(K,dA)$, where $dA$ is planar area on the two closed disks, and let $T$ multiply by $z$. Its adjoint multiplies by $\overline z$, so it is a [normal operator](../../../../../normal-operator.md). An [eigenvector](../../../../../eigenvector.md) for $\lambda$ would be supported on the area-zero singleton $\{\lambda\}$, hence would be zero in $L^2$. Outside $K$, multiplication by $1/(z-\lambda)$ is a bounded inverse to $T-\lambda I$. For $\lambda\in K$, normalized [indicator functions](../../../../../indicator-function.md) of $K\cap\{|z-\lambda|<\varepsilon\}$ have $\|(T-\lambda I)h\|\le\varepsilon$, excluding a bounded inverse. Thus its [spectrum](../../../../../spectrum-functional-analysis.md) is exactly $K$. The [linear projection](../../../../../projection-linear-algebra.md) in the figure multiplies by $\mathbf1_{K_1}$, and its range consists of functions supported on the left disk.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
