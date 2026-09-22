<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep the coordinates and operator $D_k$ from part (a). The attenuation $f$ is known, and the source $g$ is to be reconstructed. Put $F(\rho,\tau,\theta)=\int_\tau^\infty f(s\cos\theta-\rho\sin\theta,s\sin\theta+\rho\cos\theta)ds$ and $S(\rho,\theta)=\mathcal Rf=\int_{\mathbb R}f\,d\tau$. The directed forward [attenuated Radon transform](../../../../../../attenuated-radon-transform.md), for a detector at the positive end of the line, is

$$
\boxed{\mathcal A_f g(\rho,\theta)=A_f(\rho,\theta)=\int_{-\infty}^\infty e^{-F(\rho,\tau,\theta)}g(\tau\cos\theta-\rho\sin\theta,\tau\sin\theta+\rho\cos\theta)d\tau.}
$$

This weight accounts for absorption from each emission point to the detector. It is also derived by solving the real transport equation $\partial_\tau u+fu=g$ with zero incoming intensity: its outgoing limit is $A_f$. In particular reversing the line direction generally changes the measurement. The pair reconstructs $g$ from full directed data and known $f$; it does not infer both unknown functions from the same data.

We must specify the sign convention for the projectors. Use the [Hilbert transform](../../../../../../hilbert-transform.md) $Hv(\rho)=\pi^{-1}\operatorname{PV}\int_{\mathbb R}v(s)/(\rho-s)ds$ and the [signed Cauchy boundary operators](../../../../../../signed-cauchy-boundary-operators.md)

$$
P^\pm v=\pm\frac12v+\frac{i}{2}Hv.
$$

Then $P^+-P^-=I$, and the positive idempotent projectors are $P^+$ and $-P^-$. This is the signed boundary-value convention in the given limits of $M$. To express everything with ordinary complementary projectors, one may instead write $\Pi_+=P^+$, $\Pi_-=-P^-$. The given limits become

$$
M^+=-P^-S-F=:a_+-F,\qquad M^-=P^+S-F=:a_--F.
$$

Both $a_\pm$ depend on the transverse coordinate and direction but are constant along $\tau$.

The equation $D_kM=f$ supplies an [integrating factor](../../../../../../integrating-factor.md):

$$
D_k(e^M\mu)=e^M g,\qquad\mu=e^{-M}T_k(e^Mg),
$$

where $T_k$ is the inverse of unattenuated complex transport, normalized to vanish at spatial infinity. To see the normalization and analyticity rather than assume them, let $w=x_1+ix_2$. The [complexified transport Cauchy kernel](../../../../../../complexified-transport-cauchy-kernel.md) is

$$
E_k(w)=\frac{\operatorname{sgn}(1-|k|^2)}{\pi}\frac{k}{w-k^2\bar w},\qquad T_kh=E_k*h,\qquad0<|k|\ne1.
$$

In the rotated coordinates, $E_k=[2\pi|B|(\tau+iA\rho/B)]^{-1}$. The identity $\partial_{\bar z}(1/(\pi z))=\delta$ and the Jacobian $A/|B|$ prove $D_kE_k=\delta$ with exactly this normalization. The denominator cannot vanish for nonzero real $w$ off the unit circle. The kernel is analytic separately inside and outside that circle, is $O(k)$ at zero and $O(k^{-1})$ at infinity. Thus $M=T_kf$ and the displayed $\mu$ have the corresponding spectral behavior for the smooth decaying data. In particular $\mu=O(k^{-1})$ at infinity and is bounded, indeed $O(k)$, at zero.

The limiting unattenuated inverse on any smooth decaying input $h$ is

$$
T_+h=-P^-\mathcal Rh-\int_\tau^\infty h\,ds,\qquad T_-h=P^+\mathcal Rh-\int_\tau^\infty h\,ds.
$$

One may verify this directly in the rotated Fourier variables: $D_k$ has multiplier $iA\xi-B\eta$, so its inverse has a pole at $\xi=-iB\eta/A$. As $B\to0^+$, the positive transverse frequencies have the negative tail primitive and the negative transverse frequencies have the positive past primitive; for $B\to0^-$ these allocations reverse. Splitting with the Fourier projectors $\Pi_\pm$ yields exactly the two formulas above. Applying them to $f$ reproduces the assumed limits of $M$ and checks the signs.

Now apply the same limiting inverse to $h=e^{M^\pm}g$. Because $a_\pm$ are independent of $\tau$, its line integral is $e^{a_\pm}A_f$, while its tail is $e^{a_\pm}\int_\tau^\infty e^{-F}g\,ds$. Hence

$$
\begin{aligned}
\mu^+&=-e^{F-a_+}P^-(e^{a_+}A_f)-e^F\int_\tau^\infty e^{-F}g\,ds,\\
\mu^-&=e^{F-a_-}P^+(e^{a_-}A_f)-e^F\int_\tau^\infty e^{-F}g\,ds.
\end{aligned}
$$

The unknown incomplete line integral cancels in their difference. All remaining quantities are obtained from the measurements and known attenuation:

$$
\mu^+-\mu^-=-J,\qquad J=e^F\left[e^{P^-S}P^-(e^{-P^-S}A_f)+e^{-P^+S}P^+(e^{P^+S}A_f)\right].
$$

Each projection acts in $\rho$ at fixed $\theta$, before evaluating $\rho=-x_1\sin\theta+x_2\cos\theta$ and $\tau=x_1\cos\theta+x_2\sin\theta$. Pulling a transverse-dependent exponential outside a projector would be incorrect.

The sectionally analytic $\mu$ therefore solves an additive [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md) on the counterclockwise unit circle, with the plus value inside. The normalized [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) is

$$
\mu(x,k)=-\frac1{2\pi}\int_0^{2\pi}\frac{e^{i\theta}J(x,\theta)}{e^{i\theta}-k}d\theta.
$$

The [Sokhotski–Plemelj theorem](../../../../../../sokhotski-plemelj-theorem.md) gives its jump; boundedness at zero and decay at infinity make it unique by the [Liouville theorem](../../../../../../liouville-theorem.md). Its expansion at infinity is

$$
\mu(x,k)=\frac1{2\pi k}\int_0^{2\pi}e^{i\theta}J(x,\theta)d\theta+O(k^{-2}).
$$

Substitute into the original equation. The $k\partial_{x_1}-ik\partial_{x_2}$ part contributes at order one, the reciprocal derivative and $f\mu$ vanish at that order. This derives the [projection formula for inverse attenuated Radon transform](../../../../../../projection-formula-for-inverse-attenuated-radon-transform.md):

$$
\boxed{g(x_1,x_2)=\frac1{4\pi}(\partial_{x_1}-i\partial_{x_2})\int_0^{2\pi}e^{i\theta}J(x_1,x_2,\theta)d\theta.}
$$

Together with the boxed forward transform this is the requested pair. The derivation uses no small-attenuation approximation. For smooth compactly supported data the operations above are justified directly; sufficient integrable decay permits the same limiting construction.

As a normalization check, set $f=0$. Then $S=F=0$, $A_f=\mathcal Rg$ and $J=(P^-+P^+)\mathcal Rg=iH\mathcal Rg$. Since the line transform is independent of $\tau$ and $e^{i\theta}(\partial_{x_1}-i\partial_{x_2})=\partial_\tau-i\partial_\rho$, the formula reduces to

$$
g(x)=\frac1{4\pi}\int_0^{2\pi}\partial_\rho H\mathcal Rg(\rho,\theta)\big|_{\rho=x\cdot(-\sin\theta,\cos\theta)}d\theta,
$$

the full-angle inverse [Radon transform](../../../../../../radon-transform.md). For the radial Gaussian $g=e^{-|x|^2}$, $\mathcal Rg=\sqrt\pi e^{-\rho^2}$ and $\partial_\rho H\mathcal Rg(0)=2$, so the reconstructed value at the origin is $1$, checking the $1/(4\pi)$ factor.

In [single-photon emission computed tomography](../../../../../../single-photon-emission-computed-tomography.md), $g$ represents the internal emission density, $f$ the known absorption coefficient and $A_f$ the directed detector counts. Each path integral weights a source point by its survival probability to the detector. Thus the [attenuated Radon transform](../../../../../../attenuated-radon-transform.md) is the forward measurement model and its derived inverse reconstructs the emission distribution, providing the mathematical basis of [SPECT](../../../../../../single-photon-emission-computed-tomography.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
