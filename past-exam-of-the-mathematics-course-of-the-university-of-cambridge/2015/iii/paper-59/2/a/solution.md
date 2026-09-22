<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $z$ increase outward and define the inward [optical depth](../../../../../../optical-depth.md) by $d\tau/dz=-\bar\kappa\rho$. With constant outward internal [radiative flux](../../../../../../radiative-flux.md) $F=\sigma T_{\rm int}^4$, [radiative diffusion](../../../../../../radiative-diffusion.md) gives

$$
\frac{dT}{d\tau}=\frac{3F}{16\sigma T^3},\qquad \frac{dT^4}{d\tau}=\frac34T_{\rm int}^4,\qquad T^4=\frac34T_{\rm int}^4(\tau+q).
$$

The constant $q$ is a boundary condition; diffusion alone does not determine it. For an unirradiated [grey atmosphere](../../../../../../grey-atmosphere.md) with the [Eddington closure approximation](../../../../../../eddington-closure-approximation.md) and [Eddington surface boundary condition](../../../../../../eddington-surface-boundary-condition.md), $q=2/3$, so

$$
\boxed{T(\tau)=T_{\rm int}\left[\frac34\left(\tau+\frac23\right)\right]^{1/4}.}
$$

The [internal effective temperature of a planet](../../../../../../internal-effective-temperature-of-a-planet.md) is defined by its intrinsic cooling flux, not by its incident stellar heating. Since $dT/d\tau>0$ and $d\tau/dz<0$, temperature decreases outward. Towards the thin upper layers, $T\to2^{-1/4}T_{\rm int}\simeq0.84T_{\rm int}$; if the density and optical-depth gradient vanish there, $dT/dz\to0$. This is the upper nearly [isothermal atmosphere](../../../../../../isothermal-atmosphere.md). The diffusion approximation itself fails at small optical depth: the grey boundary closure supplies the approximate continuation. Small irradiation perturbs this intrinsic-flux solution.

Young, self-luminous [gas giants](../../../../../../gas-giant.md) at wide orbital separations can have intrinsic cooling dominate their photospheric budget. They are favorable for [exoplanet direct imaging](../../../../../../exoplanet-direct-imaging.md), especially in the [infrared](../../../../../../infrared.md), where their own thermal radiation is easier to separate from the host light. A strongly irradiated [hot Jupiter](../../../../../../hot-jupiter.md) instead has a large stable outer radiative region set mainly by stellar heating; it can be nearly isothermal over a broad pressure range or develop an [atmospheric thermal inversion](../../../../../../inversion-meteorology.md) if stellar light is absorbed sufficiently high. Inversion is not inevitable for every strongly irradiated planet. Deep [convection](../../../../../../convection.md) begins below its [radiative-convective boundary](../../../../../../radiative-convective-boundary.md).

<a id="2/a/image-intrinsic-grey-atmosphere-cooling-profile-compared-with-illustrative-irradiated-hot-jupiter-profiles"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59-temperature.png)

**[Figure 2](#2/a/image-intrinsic-grey-atmosphere-cooling-profile-compared-with-illustrative-irradiated-hot-jupiter-profiles). Intrinsic grey-atmosphere cooling profile compared with illustrative irradiated hot-Jupiter profiles**.

The intrinsic curve follows the grey formula. The irradiated curves illustrate possible shapes only; they are not solutions for a specified [opacity](../../../../../../opacity.md) model. Smaller optical depth corresponds to greater altitude.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
