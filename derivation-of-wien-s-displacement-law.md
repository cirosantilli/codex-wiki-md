<h1 id="derivation-of-wien-s-displacement-law">Derivation of Wien's displacement law</h1>

↑ **Parent:** [Wien's displacement law](wien-s-displacement-law.md)

At fixed $T>0$, substitute $x=hc/(\lambda k_BT)>0$ into the [Planck function](planck-function.md):

$$
B_\lambda(T)=\frac{2k_B^5T^5}{h^4c^3}\frac{x^5}{e^x-1}.
$$

Here $h$ is the [Planck constant](planck-constant.md), $k_B$ the [Boltzmann constant](boltzmann-constant.md), and $c$ the [speed of light](speed-of-light.md). Since $dx/d\lambda=-x/\lambda\ne0$, an interior maximum in [wavelength](wavelength.md) is also a stationary point in $x$. A [logarithmic derivative](logarithmic-derivative.md) gives

$$
\frac{d}{dx}\log\frac{x^5}{e^x-1}=\frac5x-\frac1{1-e^{-x}}=0,
\qquad x=5(1-e^{-x}).
$$

The required positive root is $x_\lambda=4.9651142317\ldots$. The rearranged equation also has $x=0$, but that endpoint is not a peak. For $g(x)=5(1-e^{-x})-x$, $g'(x)=5e^{-x}-1$ changes sign once, at $x=\log5$. Thus $g$ first increases and then decreases to negative values, crossing zero exactly once for $x>0$. Since $x^5/(e^x-1)$ tends to zero at both endpoints, this stationary point is the unique global maximum. Solving the definition of $x$ for [wavelength](wavelength.md) gives

$$
\lambda_{\max}=\frac{hc}{k_BTx_\lambda},\qquad b=\frac{hc}{k_Bx_\lambda}.
$$

The inverse-[temperature](temperature-split.md) dependence follows before any numerical root-finding. More generally $B_\lambda(T)=T^5F(\lambda T)$ for one fixed function $F$, so spectra at all [temperatures](temperature-split.md) have the same rescaled shape. This is stronger than a relation between two peak positions. Replacing the denominator by $e^x$ in the [Wien approximation](wien-approximation.md) would instead give $x=5$ and a peak [wavelength](wavelength.md) about $0.70\%$ too short.

## ↑ Ancestors (7)

1. [Wien's displacement law](wien-s-displacement-law.md)
2. [Planck function](planck-function.md)
3. [Radiative transfer](radiative-transfer.md)
4. [Astrophysics](astrophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Frequency form of Wien's displacement law](frequency-form-of-wien-s-displacement-law.md)
