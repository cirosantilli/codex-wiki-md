<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We place the definitions and the unheaded preliminary requests here before addressing the first labelled property. The [Schwartz space](../../../../../../schwartz-space.md) consists of [smooth functions](../../../../../../smooth-function.md) with finite [seminorms](../../../../../../seminorm.md)

$$
q_{\alpha,\beta}(f)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta f(x)|
$$

for every pair of [multi-indices](../../../../../../multi-index-notation.md). Convergence means convergence in each [seminorm](../../../../../../seminorm.md). The [tempered distribution](../../../../../../tempered-distribution.md) space $\mathcal S'(\mathbb R^n)$ is its [continuous dual space](../../../../../../continuous-dual-space-split.md), with weak convergence tested against every [Schwartz function](../../../../../../schwartz-function.md). A continuous functional satisfies a bound by finitely many of these [seminorms](../../../../../../seminorm.md), equivalently by one sufficiently large weighted [derivative](../../../../../../derivative.md) [seminorm](../../../../../../seminorm.md).

Use the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx,\qquad f(x)=\frac1{(2\pi)^n}\int e^{ix\cdot\xi}\widehat f(\xi)\,d\xi.
$$

Differentiation under the integral and [integration by parts](../../../../../../integration-by-parts.md) express $\xi^\alpha\partial_\xi^\beta\widehat f$ as a constant of modulus one times the [Fourier transform](../../../../../../fourier-transform.md) of $\partial_x^\alpha(x^\beta f)$. Its supremum is bounded by the $L^1$ norm of that function. For $s>n$, this norm is at most a constant times finitely many Schwartz [seminorms](../../../../../../seminorm.md), using the integrable weight $(1+|x|)^{-s}$. Thus $\mathcal F:\mathcal S\to\mathcal S$ is continuous.

For completeness, [Fourier inversion](../../../../../../fourier-inversion-theorem.md) follows by inserting $e^{-\varepsilon|\xi|^2}$ in the inverse integral and using [Fubini's theorem](../../../../../../fubini-s-theorem.md). The result is [convolution](../../../../../../convolution.md) with the [Gaussian approximate identity](../../../../../../gaussian-approximate-identity.md)

$$
(4\pi\varepsilon)^{-n/2}e^{-|x|^2/(4\varepsilon)}.
$$

It tends to $f$, while integrability of $\widehat f$ allows the damping factor to be removed by [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). Consequently $\mathcal F^2f=(2\pi)^nf(-\cdot)$. Reflection preserves every Schwartz [seminorm](../../../../../../seminorm.md), so the inverse transform is continuous as well. This proves **the [Fourier transform isomorphism of the Schwartz space](../../../../../../fourier-transform-isomorphism-of-the-schwartz-space.md)**.

Define the [Fourier transform of a tempered distribution](../../../../../../fourier-transform-of-a-tempered-distribution.md) by transposition,

$$
\langle\widehat u,\psi\rangle=\langle u,\widehat\psi\rangle.
$$

The Schwartz-space continuity just proved makes this a [tempered distribution](../../../../../../tempered-distribution.md). Its inverse is $(2\pi)^{-n}\mathcal R\mathcal F$, where $\langle\mathcal Ru,\psi\rangle=\langle u,\psi(-\cdot)\rangle$. These maps are continuous for weak convergence, since each pairing is a pairing with a fixed transformed test. They are also continuous for the [strong dual topology](../../../../../../strong-dual-topology.md), because the Schwartz-space maps take bounded sets to bounded sets.

The [convolution of a tempered distribution with a Schwartz function](../../../../../../convolution-of-a-tempered-distribution-with-a-schwartz-function.md) is

$$
(u*\varphi)(x)=\langle u_y,\varphi(x-y)\rangle.
$$

Smooth dependence of translated Schwartz functions gives $\partial^\alpha(u*\varphi)(x)=\langle u,\partial^\alpha\varphi(x-\cdot)\rangle$. The finite-[seminorm](../../../../../../seminorm.md) estimate and $1+|y|\leq(1+|x|)(1+|x-y|)$ show that each [derivative](../../../../../../derivative.md) has at most [polynomial growth](../../../../../../polynomial-growth.md). In particular, $u*\varphi$ is a [smooth function](../../../../../../smooth-function.md) defining a [tempered distribution](../../../../../../tempered-distribution.md). It need not itself be a [Schwartz function](../../../../../../schwartz-function.md); for example $1*\varphi=\int\varphi$.

Writing $\check\varphi(y)=\varphi(-y)$, its distributional pairing is $\langle u*\varphi,\psi\rangle=\langle u,\check\varphi*\psi\rangle$. The inner [convolution](../../../../../../convolution.md) is a [Schwartz function](../../../../../../schwartz-function.md), and this identity follows by integration in the Schwartz topology, justified by the weighted [seminorm](../../../../../../seminorm.md) estimates. A direct [Fubini's theorem](../../../../../../fubini-s-theorem.md) calculation gives $\check\varphi*\widehat\psi=\mathcal F(\widehat\varphi\psi)$. Hence

$$
\langle\widehat{u*\varphi},\psi\rangle=\langle u,\mathcal F(\widehat\varphi\psi)\rangle=\langle\widehat u,\widehat\varphi\psi\rangle,
\qquad\boxed{\widehat{u*\varphi}=\widehat u\,\widehat\varphi.}
$$

Multiplication is well defined because multiplication by $\widehat\varphi$ acts continuously on $\mathcal S$.

Now write the [Hilbert transform](../../../../../../hilbert-transform.md) as [convolution](../../../../../../convolution.md) with $K=\pi^{-1}\operatorname{pv}(1/x)$, the [principal-value reciprocal distribution](../../../../../../principal-value-reciprocal-distribution.md). The given [Heaviside function](../../../../../../heaviside-step-function.md) transform, together with $\mathcal F^2H=2\pi H(-\cdot)$, yields

$$
\pi-i\mathcal F\big(\operatorname{pv}(1/x)\big)=2\pi H(-\xi),\qquad\widehat K(\xi)=-i\operatorname{sgn}\xi.
$$

The value of the sign function at zero is irrelevant to its regular [distribution](../../../../../../distribution-mathematical-analysis.md). Thus the [Hilbert-transform Fourier multiplier](../../../../../../hilbert-transform-fourier-multiplier.md) is

$$
\widehat{\mathcal H\varphi}(\xi)=-i\operatorname{sgn}(\xi)\widehat\varphi(\xi).
$$

Applying [Plancherel theorem](../../../../../../plancherel-theorem.md), whose normalization here is $\|f\|_2^2=(2\pi)^{-1}\|\widehat f\|_2^2$, proves **the isometry**:

$$
\boxed{\|\mathcal H\varphi\|_{L^2}=\|\varphi\|_{L^2}.}
$$

The principal-value integral agrees with this [convolution](../../../../../../convolution.md): near its singular point subtract $\varphi(x)$, and use odd cancellation; at infinity the Schwartz decay gives convergence. The [Hilbert transform](../../../../../../hilbert-transform.md) has domain $\mathcal S$, but generally does not take values in $\mathcal S$, as the tail in part (c) demonstrates.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
