<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For unresolved, uniformly bright [blackbodies](../../../../../../blackbody.md) at a common distance $d$, the monochromatic observed [radiative fluxes](../../../../../../radiative-flux.md) are $F_{s,\lambda}=\pi B_\lambda(T_s)R_s^2/d^2$ and $F_{p,\lambda}=\pi B_\lambda(T_p)R_p^2/d^2$. Define the planet-star contrast $r_\lambda=F_{p,\lambda}/F_{s,\lambda}$. The [Planck law](../../../../../../planck-s-law.md) gives

$$
r_\lambda=\left(\frac{R_p}{R_s}\right)^2\frac{e^{hc/(\lambda k_BT_s)}-1}{e^{hc/(\lambda k_BT_p)}-1}.
$$

Outside the [exoplanet secondary eclipse](../../../../../../exoplanet-secondary-eclipse.md), the system flux is $F_s+F_p$; during complete occultation it is $F_s$. Consequently the exact [thermal eclipse depth](../../../../../../thermal-eclipse-depth.md) normalized to the out-of-eclipse light is

$$
\boxed{d_\lambda=\frac{F_{p,\lambda}}{F_{s,\lambda}+F_{p,\lambda}}=\frac{r_\lambda}{1+r_\lambda}.}
$$

Only in the faint-planet limit is $d_\lambda\simeq r_\lambda$. Reflected starlight, partial occultation and spatial temperature variations are omitted under the stated [blackbody](../../../../../../blackbody.md) model.

For a cooler [hot Jupiter](../../../../../../hot-jupiter.md) with $T_p<T_s$, the planet-star contrast is exponentially small at short wavelengths and increases towards a constant plateau. This is the [monotonicity of blackbody planet-star contrast](../../../../../../monotonicity-of-blackbody-planet-star-contrast.md), rather than the peaked shape of the planet's absolute [blackbody](../../../../../../blackbody.md) flux. An illustrative example uses $T_p=1500\,\mathrm K$, $T_s=5800\,\mathrm K$ and $R_p/R_s=0.1$:

<a id="1/b/image-blackbody-hot-jupiter-planet-star-contrast-increasing-towards-its-rayleigh-jeans-plateau"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59-contrast.png)

**[Figure 1](#1/b/image-blackbody-hot-jupiter-planet-star-contrast-increasing-towards-its-rayleigh-jeans-plateau). Blackbody hot-Jupiter planet-star contrast increasing towards its Rayleigh-Jeans plateau**.

At wavelengths long enough for the [Rayleigh-Jeans law](../../../../../../rayleigh-jeans-law.md) to apply to both bodies, $B_\lambda\simeq2ck_BT/\lambda^4$. Therefore

$$
\boxed{r_\lambda\longrightarrow r_\infty=\left(\frac{R_p}{R_s}\right)^2\frac{T_p}{T_s},\qquad d_\lambda\longrightarrow\frac{r_\infty}{1+r_\infty}.}
$$

The common $\lambda^{-4}$ dependence cancels. In the illustrative case, the contrast plateau is about $2.6\times10^{-3}$, or $2600$ parts per million.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
