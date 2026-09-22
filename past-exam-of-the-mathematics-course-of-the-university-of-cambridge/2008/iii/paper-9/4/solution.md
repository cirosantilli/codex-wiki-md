<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix [Haar measure](../../../../../haar-measure.md) $m_G$ and use $\widehat f(\chi)=\int_G f(x)\overline{\chi(x)}\,dm_G(x)$. A [positive-definite function](../../../../../positive-definite-function.md) $p$ satisfies $\sum_{i,j}z_i\overline{z_j}p(x_i-x_j)\geq0$ for every finite choice of points and coefficients. The [Bochner theorem](../../../../../bochner-s-theorem.md) states that a continuous positive-definite function on a locally compact Hausdorff Abelian group has a unique representation

$$
\boxed{p(x)=\int_{\widehat G}\chi(x)\,d\mu_p(\chi),\qquad \mu_p\geq0,\qquad\mu_p(\widehat G)=p(0)<\infty,}
$$

where $\mu_p$ is a [Radon measure](../../../../../radon-measure.md). Conversely, any finite positive [Radon measure](../../../../../radon-measure.md) on the [Pontryagin dual group](../../../../../pontryagin-dual-group.md) has a continuous positive-definite inverse transform. The sign convention here is the one compatible with the displayed Fourier transform.

First note that the dual is a locally compact Hausdorff [topological group](../../../../../topological-group-split.md). Its group operations are continuous in the [compact-open topology](../../../../../compact-open-topology.md) proved in question 3. For local compactness, adjoin the zero functional to the [character space of an algebra](../../../../../character-space-of-an-algebra.md) of $L^1(G)$. All its elements lie in the closed unit ball of $L^1(G)^*$, and the equations $\varphi(a*b)=\varphi(a)\varphi(b)$ define a closed subset in the [weak-star topology](../../../../../weak-star-topology.md). The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes that subset compact Hausdorff. Removing the zero functional gives an open, hence locally compact, subspace. This provides the setting for constructing the measure on the dual, without assuming a [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md).

Let $u^*(x)=\overline{u(-x)}$ and let $\mathcal P$ be the finite sums of convolution squares $u*u^*$, $u\in C_c(G)$. Each such square is continuous with [compact support](../../../../../compact-support.md), and is positive-definite because

$$
\sum_{i,j}z_i\overline{z_j}(u*u^*)(x_i-x_j)=\int_G\left|\sum_i z_i u(t+x_i)\right|^2dm_G(t)\geq0.
$$

Its transform is $|\widehat u|^2$, so every $p\in\mathcal P$ has $\widehat p\geq0$. Also $p*q\in\mathcal P$: convolution of two squares is $(u*v)*(u*v)^*$, and finite sums distribute. Insert the Bochner representation of $q$ into $p*q$ and use the [Fubini theorem](../../../../../fubini-s-theorem.md) to obtain

$$
(p*q)(x)=\int_{\widehat G}\chi(x)\widehat p(\chi)\,d\mu_q(\chi).
$$

The representing measure on the right is finite and positive. Uniqueness in the [Bochner theorem](../../../../../bochner-s-theorem.md) and commutativity now give the [Bochner consistency identity for convolution squares](../../../../../bochner-consistency-identity-for-convolution-squares.md)

$$
\widehat p\,\mu_q=\widehat q\,\mu_p=\mu_{p*q}.
$$

For every compact $K\subseteq\widehat G$ there is $p\in\mathcal P$ with $\widehat p>0$ throughout $K$. Indeed, at any $\chi_0$ choose $u=\chi_0 a$, where $a\geq0$ is a nonzero member of $C_c(G)$. Then $\widehat u(\chi_0)=\int a>0$, and continuity supplies a neighbourhood where it stays nonzero. A finite subcover of $K$ and the sum of the corresponding squares give such a $p$.

For $\psi\in C_c(\widehat G)$, choose $p$ positive in transform on its support and define

$$
J(\psi)=\int_{\widehat G}\frac{\psi(\chi)}{\widehat p(\chi)}\,d\mu_p(\chi).
$$

The quotient is set to zero away from the support; its denominator is bounded away from zero there. If $q$ is another choice, the consistency identity, multiplied by $\psi/(\widehat p\widehat q)$ on that [compact support](../../../../../compact-support.md), shows that the integral is unchanged. Choosing one $p$ for a union of supports proves linearity; positivity follows from positivity of $\mu_p$. On each fixed [compact support](../../../../../compact-support.md) it is bounded by $\mu_p(K)/\min_K\widehat p$ times the uniform norm. Moreover, for every $p\in\mathcal P$ and $\psi\in C_c(\widehat G)$, choosing $q$ positive on the support of $\psi$ gives

$$
J(\psi\widehat p)=\int\frac{\psi\widehat p}{\widehat q}\,d\mu_q=\int\psi\,d\mu_p.
$$

A nonzero square has $\mu_p(\widehat G)=p(0)=\|u\|_2^2>0$; a suitable nonnegative [compactly supported](../../../../../compact-support.md) $\psi$ consequently makes this last expression positive. Thus $J$ is nonzero.

To prove translation invariance, fix $\eta\in\widehat G$ and modulate $p$ by $p_\eta(x)=\eta(x)p(x)$. This again belongs to $\mathcal P$, since modulation takes $u*u^*$ to $(\eta u)*(\eta u)^*$. Direct calculation and Bochner uniqueness give

$$
\widehat{p_\eta}(\chi)=\widehat p(\eta^{-1}\chi),\qquad\mu_{p_\eta}=(T_\eta)_*\mu_p,\qquad T_\eta(\chi)=\eta\chi.
$$

Hence, for $\psi_\eta(\chi)=\psi(\eta^{-1}\chi)$, using $p_\eta$ as the denominator function and changing variables gives $J(\psi_\eta)=J(\psi)$. The [Riesz representation on compactly supported continuous functions](../../../../../riesz-representation-on-compactly-supported-continuous-functions.md) now produces a nonzero translation-invariant positive [Radon measure](../../../../../radon-measure.md) $\nu$ on the dual. It is finite on compact sets, so it is [Haar measure](../../../../../haar-measure.md). This is the compatible [dual Haar measure](../../../../../dual-haar-measure.md), denoted $m_{\widehat G}=\nu$.

The identity for $J(\psi\widehat p)$ says, by uniqueness of [Radon measures](../../../../../radon-measure.md),

$$
d\mu_p=\widehat p\,d\nu.
$$

Thus $\widehat p\in L^1(\widehat G,\nu)$ and the Bochner representation immediately proves

$$
p(x)=\int_{\widehat G}\widehat p(\chi)\chi(x)\,d\nu(\chi)\qquad(p\in\mathcal P).
$$

It also proves the formula for all finite complex linear combinations of these functions. The measure scale is fixed by this identity: at $x=0$, a nonzero square gives $\int|\widehat u|^2d\nu=\|u\|_2^2$.

A wider inversion class is $f\in L^1(G)$ with $\widehat f\in L^1(\widehat G,\nu)$. To prove this extension, choose nonnegative $a_U\in C_c(G)$ with integral one and support in a small identity neighbourhood $U$, and put $p_U=a_U*a_U^*$. These functions form an [approximate identity](../../../../../approximate-identity.md): they are nonnegative, have integral one and support in $U-U$. Also $0\leq\widehat p_U=|\widehat a_U|^2\leq1$, and $\widehat p_U\to1$ uniformly on compact subsets of the dual. For this [uniform convergence](../../../../../uniform-convergence.md) use [equicontinuity of compact families of characters](../../../../../equicontinuity-of-compact-families-of-characters.md): evaluation is jointly continuous, as follows from the translation quotient in question 3, and a finite cover of a compact family gives uniform control near the identity.

Convolving the already established inversion formula for $p_U$ with $f$, the [Fubini theorem](../../../../../fubini-s-theorem.md) gives

$$
(f*p_U)(x)=\int_{\widehat G}\widehat f(\chi)\widehat p_U(\chi)\chi(x)\,d\nu(\chi).
$$

This is justified by $\|f\|_1\mu_{p_U}(\widehat G)<\infty$. Compact-set [uniform convergence](../../../../../uniform-convergence.md) and an integrable-tail split imply

$$
\int_{\widehat G}|\widehat f|\,|\widehat p_U-1|\,d\nu\longrightarrow0.
$$

Explicitly, first choose a compact set outside which $\int|\widehat f|$ is small, use the bound $|\widehat p_U-1|\leq2$ on that tail, and use [uniform convergence](../../../../../uniform-convergence.md) on the compact remainder. This argument works for neighbourhood-indexed nets, without assuming metrizability. Consequently $f*p_U$ converges uniformly to the continuous inverse integral. On the other hand, [translation continuity in Lp on a locally compact group](../../../../../translation-continuity-in-lp-on-a-locally-compact-group.md) gives $f*p_U\to f$ in $L^1$; testing these two limits against $C_c(G)$ shows they agree almost everywhere. At every continuity point of the chosen representative of $f$, the shrinking-support [approximate identity](../../../../../approximate-identity.md) also converges pointwise to $f(x)$. We obtain [Fourier inversion on a locally compact abelian group](../../../../../fourier-inversion-on-a-locally-compact-abelian-group.md):

$$
\boxed{f(x)=\int_{\widehat G}\widehat f(\chi)\langle x,\chi\rangle\,dm_{\widehat G}(\chi),\qquad \langle x,\chi\rangle=\chi(x),}
$$

valid everywhere for continuous $f\in L^1(G)$ with integrable transform, and in general as equality with a continuous representative almost everywhere. This class includes all convolution squares above, and their linear span.

Finally, for arbitrary $h\in C_c(G)$, apply the inversion formula at zero to $h*h^*$:

$$
\int_{\widehat G}|\widehat h(\chi)|^2\,d\nu(\chi)=(h*h^*)(0)=\int_G|h(x)|^2\,dm_G(x).
$$

Thus the integral Fourier transform is linear and norm-preserving on $C_c(G)$. That space is dense in $L^2(G)$, so for $f\in L^2(G)$ choose $h_n\in C_c(G)$ with $h_n\to f$ in $L^2$ and define $\mathcal Ff$ as the $L^2(\widehat G,\nu)$ limit of $\widehat h_n$. The norm identity makes this limit exist and independent of the approximating sequence, and preserves linearity. This proves the [Plancherel theorem for locally compact abelian groups](../../../../../plancherel-theorem-for-locally-compact-abelian-groups.md) in the requested form:

$$
\boxed{\mathcal F:L^2(G,m_G)\longrightarrow L^2(\widehat G,m_{\widehat G})\text{ is linear},\qquad\|\mathcal Ff\|_2=\|f\|_2.}
$$

On $L^1\cap L^2$, choose the approximating sequence to converge in both norms; [uniform convergence](../../../../../uniform-convergence.md) of the integral transforms and their $L^2$ convergence show that this extension agrees almost everywhere with the original transform. For general $L^2$ functions the extension is defined by norm limits, not by presuming that the pointwise integral exists.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
