# Standardization of Type Ia supernova light curves

↑ **Parent:** [Type Ia supernova cosmology](type-ia-supernova-cosmology.md)

The stretch method rescales the [light curve](light-curve.md)'s time axis by $s(1+z)$ and corrects peak [apparent magnitude](apparent-magnitude.md) by $\alpha(s-1)$, fitting $\alpha$ jointly with cosmology.[Section 2, equations (1)–(2): stretch and time dilation](measurements-of-omega-and-lambda-from-42-high-redshift-supernovae-by-saul-perlmutter-and-others.md)

Here is a deliberately stipulated local model that exposes the signs. Let $t_{\rm obs}$ be observer time in [days](day.md), $t_{\max}$ the observed peak time and $T(u)$ a dimensionless template with $T(0)=1$. In a single [photometric passband](photometric-passband.md), write

$$
u=\frac{t_{\rm obs}-t_{\max}}{s(1+z)},\qquad F(t_{\rm obs})=F_{\max}T(u).
$$

Here $u$ is rest-frame time in [days](day.md); the template's argument carries those units. For illustration, assign the intrinsic relation $M_B(s)=M_{B,0}-\alpha(s-1)$ with $\alpha>0$: broader events are intrinsically brighter. Define the sign of the [K correction](k-correction.md) by $m_{\rm obs}=M_B(s)+\mu+A_B+K$, where $A_B$ is [interstellar extinction](interstellar-extinction.md) in magnitudes. Then

$$
m_{B,\rm corr}=m_{\rm obs}-K-A_B+\alpha(s-1)=M_{B,0}+\mu.
$$

Removing attenuation makes the magnitude smaller; standardizing a broad, intrinsically bright event makes it larger. The fitted [cosmological time dilation](cosmological-time-dilation.md) must be removed before comparing intrinsic durations. This schematic factorization explains the bookkeeping; an actual multicolour fit must also model changing intrinsic colours and correlated uncertainties.

For two equally standardized sources, cancellation of their common [absolute magnitude](absolute-magnitude.md) gives an especially clean result:

$$
\mu_2-\mu_1=m_{B,\rm corr,2}-m_{B,\rm corr,1},\qquad
\frac{d_{L,2}}{d_{L,1}}=10^{(\mu_2-\mu_1)/5}.
$$

A stipulated residual of $+0.20$ mag therefore means a distance ratio $10^{0.04}=1.09648$ and a [radiative flux](radiative-flux.md) ratio $10^{-0.08}=0.83176$ relative to the comparison prediction, provided [luminosity](luminosity.md) and attenuation have been correctly standardized. This is a conversion of a hypothetical residual, not a measured survey value.

## ↑ Ancestors (6)

1. [Type Ia supernova cosmology](type-ia-supernova-cosmology.md)
2. [Luminosity distance](luminosity-distance.md)
3. [Cosmology](cosmology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
