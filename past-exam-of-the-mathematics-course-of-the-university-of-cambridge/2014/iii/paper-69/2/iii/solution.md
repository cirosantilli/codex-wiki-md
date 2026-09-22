<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume for this spectral construction that the source and known attenuation are sufficiently smooth and decaying, for instance compactly supported, and that $\mu\geq0$ for the physical interpretation. The following steps identify both the forward [attenuated Radon transform](../../../../../../attenuated-radon-transform.md) and the route to its inversion.

First write the complex transport operator as

$$
L_k=k\partial_z+k^{-1}\partial_{\bar z}.
$$

For $k=e^{i\theta}$ this is the real directional derivative $\boldsymbol d_\theta\cdot\nabla$, with $\boldsymbol d_\theta=(\cos\theta,\sin\theta)$. Put $\boldsymbol n_\theta=(-\sin\theta,\cos\theta)$ and $x=p\boldsymbol n_\theta+s\boldsymbol d_\theta$. The spectral equation on the [unit circle](../../../../../../complex-unit-circle.md) becomes

$$
\partial_sF-\mu(p,s)F=f(p,s).
$$

Its minus sign fixes the appropriate endpoint condition: use $F(p,+\infty)=0$. The [integrating factor](../../../../../../integrating-factor.md) gives

$$
F(p,s)=-\int_s^\infty
\exp\left[-\int_s^r\mu(p,v)\,dv\right]f(p,r)\,dr.
$$

Thus the measured quantity at the opposite end of the line is

$$
\boxed{\mathcal R^-_\mu f(p,\theta)
=-F(p,-\infty)=\int_{-\infty}^\infty
f(p\boldsymbol n_\theta+s\boldsymbol d_\theta)
\exp\left[-\int_{-\infty}^{s}\mu(p\boldsymbol n_\theta+r\boldsymbol d_\theta)\,dr\right]ds.}
$$

The exponent is the attenuation accumulated between the source point and the detector at the negative end. The common convention with detector at the positive end is the same transform after reversing the direction, $\mathcal R^+_\mu f(p,\theta)=\mathcal R^-_\mu f(-p,\theta+\pi)$. Using an incoming zero condition at the negative end while retaining the printed minus sign would instead give a growing integrating factor, not physical attenuation.

Next, for $|k|\ne1$, the operator $L_k$ is a complex elliptic first-order operator. Its decaying whole-plane [Green function](../../../../../../green-s-function.md) is

$$
G_k(z)=\frac{\operatorname{sgn}(|k|^2-1)}{\pi(k\bar z-k^{-1}z)},\qquad L_kG_k=\delta_0.
$$

This is obtained by a real-linear change of variables in the [Cauchy-Green operator](../../../../../../cauchy-green-operator.md); its change of orientation explains the sign. Write $G_k a$ for convolution with this kernel. Solve $L_kh=\mu$, and set $F=e^h\Psi$. This removes the attenuation:

$$
L_k\Psi=e^{-h}f,\qquad h=G_k\mu,\qquad \Psi=G_k(e^{-h}f).
$$

The normalized spectral solution is analytic separately inside and outside the [unit circle](../../../../../../complex-unit-circle.md). As $k$ approaches that circle, the [Green function](../../../../../../green-s-function.md)'s characteristic singularity produces two limiting values. Their relation is computed from the weighted line integrals above together with transverse [Hilbert transforms](../../../../../../hilbert-transform.md); the known attenuation determines the [integrating factor](../../../../../../integrating-factor.md) weights. The two spectral limits are not individually just the incoming and outgoing real characteristic solutions: the singular-kernel prescription matters.

Finally formulate the resulting additive [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md) on the [unit circle](../../../../../../complex-unit-circle.md). Its jump is determined by the measured [attenuated Radon transform](../../../../../../attenuated-radon-transform.md) and known $\mu$. With the [unit circle](../../../../../../complex-unit-circle.md) oriented counterclockwise and jump $J=F_{\rm inside}-F_{\rm outside}$, a [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) reconstructs the normalized spectral solution:

$$
F(z,k)=\frac1{2\pi i}\int_{|\zeta|=1}\frac{J(z,\zeta)}{\zeta-k}\,d\zeta.
$$

The normalization at zero supplies the compatibility condition $\int J/\zeta\,d\zeta=0$. Recover $f$ from $L_kF-\mu F$, or from its small-$k$ coefficient: if $F=kF_1+O(k^2)$, then $f=\partial_{\bar z}F_1$. Equivalently the large-$k$ coefficient gives $f=\partial_zF_{-1}$ when $F=k^{-1}F_{-1}+O(k^{-2})$. This [spectral reconstruction of an attenuated Radon transform](../../../../../../spectral-reconstruction-of-an-attenuated-radon-transform.md) is the analogue of recovering $q$ from a coefficient in (ii). Known attenuation and full directed line data are inputs; one does not determine an arbitrary unknown attenuation and source simultaneously from this argument.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
