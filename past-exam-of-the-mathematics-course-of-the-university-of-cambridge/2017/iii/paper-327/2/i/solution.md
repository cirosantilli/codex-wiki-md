<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [multi-indices](../../../../../../multi-index-notation.md) $\alpha,\beta$, define

$$
p_{\alpha,\beta}(\varphi)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta\varphi(x)|,\qquad
\mathcal S(\mathbb R^n)=\{\varphi\in C^\infty:p_{\alpha,\beta}(\varphi)<\infty\ \text{for all }\alpha,\beta\}.
$$

These [seminorms](../../../../../../seminorm.md) define the [Fréchet space](../../../../../../frechet-space.md) topology of the [Schwartz space](../../../../../../schwartz-space.md): $\varphi_j\to\varphi$ exactly when every $p_{\alpha,\beta}(\varphi_j-\varphi)$ tends to zero. An equivalent increasing family is

$$
q_m(\varphi)=\max_{|\beta|\leq m}\sup_x(1+|x|)^m|\partial^\beta\varphi(x)|.
$$

A [tempered distribution](../../../../../../tempered-distribution.md) is a continuous [linear functional](../../../../../../linear-functional.md) on this space. Equivalently, $|\langle T,\varphi\rangle|\leq Cq_m(\varphi)$ for some $C,m$. The usual [weak convergence of tempered distributions](../../../../../../weak-convergence-of-tempered-distributions.md) means $\langle T_j,\varphi\rangle\to\langle T,\varphi\rangle$ for every fixed [Schwartz function](../../../../../../schwartz-function.md). The [strong dual topology](../../../../../../strong-dual-topology.md) instead requires uniform convergence on every subset of the [Schwartz space](../../../../../../schwartz-space.md) that is a [bounded set in a topological vector space](../../../../../../bounded-set-in-a-topological-vector-space.md); the Fourier maps below are continuous in both topologies.

Using $\widehat\varphi(\xi)=\int e^{-ix\cdot\xi}\varphi(x)\,dx$, differentiation under the integral and [integration by parts](../../../../../../integration-by-parts.md) give

$$
\left|\xi^\alpha\partial_\xi^\beta\widehat\varphi(\xi)\right|
\leq\left\|\partial_x^\alpha(x^\beta\varphi)\right\|_{L^1}.
$$

The omitted coefficient has modulus one. By the [Leibniz rule](../../../../../../leibniz-rule.md), every integrand is a finite sum of a polynomial times a derivative of $\varphi$. Inserting the integrable weight $(1+|x|)^{-n-1}$ bounds its [L1 norm](../../../../../../l1-norm.md) by finitely many [Schwartz space](../../../../../../schwartz-space.md) seminorms. In particular $q_m(\widehat\varphi)\leq C_mq_{m+n+1}(\varphi)$. Thus the [Fourier transform](../../../../../../fourier-transform.md) maps $\mathcal S$ continuously into itself.

For completeness, the [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) follows here by Gaussian regularization. The inverse transform of $e^{-t|\xi|^2}$ is $g_t(x)=(4\pi t)^{-n/2}e^{-|x|^2/(4t)}$. The [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md) and [Fubini's theorem](../../../../../../fubini-s-theorem.md) show

$$
(2\pi)^{-n}\int e^{ix\cdot\xi}e^{-t|\xi|^2}\widehat\varphi(\xi)\,d\xi
=(g_t*\varphi)(x).
$$

As $t\downarrow0$, the right side tends to $\varphi(x)$ by the [approximate identity](../../../../../../approximate-identity.md) property, while the left side tends to the undamped inverse integral by [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), since $\widehat\varphi\in L^1$. Hence

$$
\boxed{\mathcal F^{-1}\psi(x)=(2\pi)^{-n}\int e^{ix\cdot\xi}\psi(\xi)\,d\xi,\qquad
\mathcal F^2\varphi(x)=(2\pi)^n\varphi(-x).}
$$

The inverse is $(2\pi)^{-n}$ times reflection composed with the continuous [Fourier transform](../../../../../../fourier-transform.md), and is therefore continuous on the [Schwartz space](../../../../../../schwartz-space.md). This proves a continuous linear isomorphism with continuous inverse.

Define the [Fourier transform of a tempered distribution](../../../../../../fourier-transform-of-a-tempered-distribution.md) by

$$
\langle\widehat T,\varphi\rangle=\langle T,\widehat\varphi\rangle.
$$

The continuous map on [Schwartz space](../../../../../../schwartz-space.md) makes this a [tempered distribution](../../../../../../tempered-distribution.md); the transpose of $\mathcal F^{-1}$ supplies its inverse. Pointwise convergence of pairings proves weak continuity. For the [strong dual topology](../../../../../../strong-dual-topology.md), the transform of a bounded set of [Schwartz functions](../../../../../../schwartz-function.md) is bounded, so uniform convergence of pairings on bounded sets proves continuity of both Fourier maps there too.

Now let $R\in SO(n)$ be a [rotation matrix](../../../../../../rotation-matrix.md) in the [special orthogonal group](../../../../../../special-orthogonal-group.md) and write $\rho_RT=T\circ R$. A change of variables with unit Jacobian gives

$$
\widehat{\varphi\circ R^t}(\xi)=\widehat\varphi(R^t\xi).
$$

The [rotation equivariance of the Fourier transform](../../../../../../rotation-equivariance-of-the-fourier-transform.md) on [tempered distributions](../../../../../../tempered-distribution.md) follows by duality:

$$
\begin{aligned}
\langle\widehat{\rho_RT},\varphi\rangle
&=\langle T,\widehat\varphi\circ R^t\rangle
=\langle T,\widehat{\varphi\circ R^t}\rangle\\
&=\langle\widehat T,\varphi\circ R^t\rangle
=\langle\rho_R\widehat T,\varphi\rangle.
\end{aligned}
$$

Therefore $\widehat{\rho_RT}=\rho_R\widehat T$. Applying this identity and the inverse [Fourier transform](../../../../../../fourier-transform.md) gives the two directions:

$$
\boxed{T\circ R=T\ \text{for every }R\in SO(n)
\ \Longleftrightarrow\ \widehat T\circ R=\widehat T\ \text{for every }R\in SO(n).}
$$

This is precisely preservation of [radial tempered distributions](../../../../../../radial-tempered-distribution.md). For $n>1$, $SO(n)$ acts transitively on spheres, so an invariant smooth function is an ordinary [radial function](../../../../../../radial-function.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
