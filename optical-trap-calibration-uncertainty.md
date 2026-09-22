# Optical trap calibration uncertainty

↑ **Parent:** [Harmonic optical trap](harmonic-optical-trap.md)

Write $s_V^2$ for the detector's position-related voltage [variance](variance-split.md), after characterizing independent detector noise and the acquisition response. The [equipartition theorem](equipartition-theorem.md) estimate is $k=k_BT/(\beta^2s_V^2)$. For small independent input [standard uncertainties](standard-uncertainty.md), first-order propagation gives

$$
\left(\frac{u_k}{k}\right)^2\simeq
\left(\frac{u_T}{T}\right)^2+
4\left(\frac{u_\beta}{\beta}\right)^2+
\left(\frac{u_{s_V^2}}{s_V^2}\right)^2.
$$

In this expression $u_{s_V^2}$ is the uncertainty of the [variance](variance-split.md) itself. If the assumed independent relative uncertainties are $1\%$, $2\%$, and $3\%$, respectively, the resulting relative [standard uncertainty](standard-uncertainty.md) is $\sqrt{26}\%\simeq5.10\%$. This invented budget excludes model bias. Shared calibration inputs introduce [covariance](covariance.md) terms: a [force](force-split.md) estimate $F=k\beta\overline V$ using this same thermal estimate has $F=k_BT\overline V/(\beta s_V^2)$, so treating $k$ and $\beta$ as independent would count their sensitivity incorrectly.

Correlated [Brownian motion](brownian-motion-split.md) also makes sample count a poor proxy for independent information. For a long continuous stationary Gaussian record of duration $\mathcal T$, estimating $\sigma^2$ from $\mathcal T^{-1}\int x(t)^2dt$ gives, to leading order,

$$
\operatorname{Var}(\widehat{\sigma^2})\simeq
\frac{2\sigma^4\tau}{\mathcal T},\qquad
\frac{u_{\widehat{\sigma^2}}}{\sigma^2}\simeq
\sqrt{\frac{2\tau}{\mathcal T}}.
$$

The [Gaussian distribution](normal-distribution.md) fourth-moment identity gives $\operatorname{Cov}(x(t)^2,x(0)^2)=2C_x(t)^2$; integrating this covariance over the observation interval gives the result. Subtracting a fitted mean changes higher-order terms when $\mathcal T\gg\tau$. The ideal $10\,\mathrm s$ example gives about $0.97\%$ relative uncertainty in the [variance](variance-split.md), even though $200000$ samples were recorded. This ideal statistical estimate does not include drift, detector noise or incorrect drag.

## ↑ Ancestors (6)

1. [Harmonic optical trap](harmonic-optical-trap.md)
2. [Optical tweezers](optical-tweezers.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
