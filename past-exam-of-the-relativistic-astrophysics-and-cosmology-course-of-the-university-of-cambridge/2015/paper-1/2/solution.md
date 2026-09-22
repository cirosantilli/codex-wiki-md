<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Definitions and [pressure](../../../../pressure-split.md) convention.** $R(t)$ is the [scale factor](../../../../scale-factor-cosmology.md), $t$ [cosmic time](../../../../cosmic-time.md) and dots [time derivatives](../../../../time-derivative.md). $G$ is the [gravitational constant](../../../../gravitational-constant.md), $c$ the [speed of light](../../../../speed-of-light.md), $\rho$ the mass-equivalent [density](../../../../density.md) of the material fluid and $k=+1,0,-1$ the spatial-curvature sign in this normalization. $\Lambda$ here has units of inverse time squared, rather than inverse length squared. Comparison of the acceleration equation with $\ddot R/R=\Lambda/3-4\pi G(\rho+3P/c^2)/3$ fixes

$$
\boxed{\epsilon=\frac{3P}{\rho c^2}=3w}.
$$

This $\epsilon$ is a [pressure](../../../../pressure-split.md) parameter, unrelated to Question 1's radiative efficiency. [pressureless matter](../../../../pressureless-matter.md) has $P=0$ and $\epsilon=0$. When solving the generalized model below, $\epsilon$ is assumed constant.

**Evidence for a positive vacuum component.** Standardized [Type Ia supernovae](../../../../type-ia-supernova.md) measure the luminosity-distance–[redshift](../../../../redshift.md) relation. Their corrected apparent magnitudes at cosmological distances imply greater distances than a decelerating matter-dominated model of comparable parameters, favoring late accelerated expansion. Light-curve standardization, [interstellar extinction](../../../../interstellar-extinction.md), selection bias and possible population evolution must be controlled rather than treating every supernova as an identical candle.[Abstract and distance–redshift analysis](../../../../observational-evidence-from-supernovae-for-an-accelerating-universe-and-a-cosmological-constant-by-adam-riess-and-others.md)[Abstract and cosmological likelihood analysis](../../../../measurements-of-omega-and-lambda-from-42-high-redshift-supernovae-by-saul-perlmutter-and-others.md)

The [cosmic microwave background](../../../../cosmic-microwave-background-split.md) and [baryon acoustic oscillation](../../../../baryon-acoustic-oscillation.md) measurements constrain geometry and matter [density](../../../../density.md) in combination. Near spatial flatness together with a subcritical matter [density](../../../../density.md) leaves room for an additional smooth component; cosmic ages and structure growth supply consistency tests. A positive [cosmological constant](../../../../cosmological-constant.md) fits these observations within the standard framework. They do not establish that every allowed dark-energy theory must be a strictly constant vacuum [energy](../../../../energy-split.md); the inference depends on the cosmological and gravitational model.

**[pressureless matter](../../../../pressureless-matter.md) evolution.** Set $k=0$ and $\epsilon=0$. Since $\dot H=\ddot R/R-H^2$, eliminating $\rho$ gives

$$
\dot H=-\frac32\left(H^2-\frac{\Lambda}{3}\right),\qquad
\boxed{\frac23\dot H+H^2=\frac{\Lambda}{3}}.
$$

For $H=b\coth(at)$, $\dot H=-ab\,\mathrm{csch}^2(at)$ and $\coth^2x=1+\mathrm{csch}^2x$. Therefore

$$
b^2+\left(b^2-\frac23ab\right)\mathrm{csch}^2(at)=\frac{\Lambda}{3}.
$$

On the expanding Big-Bang branch with positive $\Lambda$, choose

$$
\boxed{b=\sqrt{\frac{\Lambda}{3}},\qquad
a=\frac32b=\frac{\sqrt{3\Lambda}}2,\qquad
H(t)=\sqrt{\frac{\Lambda}{3}}
\coth\left(\frac{\sqrt{3\Lambda}}2t\right)}.
$$

The origin $t=0$ is the [Big Bang](../../../../big-bang.md); an arbitrary time translation would shift this origin. Integrating gives $R\propto\sinh^{2/3}(at)$. At early times $H\sim2/(3t)$, while at late times $H\to\sqrt{\Lambda/3}$.

**Age and the [density](../../../../density.md) fractions.** Dividing the flat constraint by $H^2$, with $\rho_{\rm crit}=3H^2/(8\pi G)$, gives

$$
\boxed{\Omega_m+\Omega_\Lambda=1,\qquad
\Omega_\Lambda=\frac{\Lambda}{3H^2}}.
$$

The solution implies $\sqrt{\Omega_\Lambda}=\tanh(at)$, so

$$
\boxed{t_0=\frac{2}{3H_0\sqrt{1-\Omega_{m0}}}
\operatorname{artanh}\sqrt{1-\Omega_{m0}}}.
$$

Here $H_0=2.3331\times10^{-18}\ \mathrm{s^{-1}}$, using the printed megaparsec conversion. Taking one year as $365.25$ days gives

$$
\boxed{t_0\simeq1.309\times10^{10}\ \mathrm{yr}=13.09\ \mathrm{Gyr}.}
$$

For the same $H_0$, an [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md) has

$$
\boxed{t_{\rm EdS}=\frac{2}{3H_0}\simeq9.05\ \mathrm{Gyr}.}
$$

A cosmic model must be older than its oldest objects, with additional time allowed for their formation. Old stellar populations are dated through stellar-evolution fitting, particularly the [globular cluster](../../../../globular-cluster.md) [main-sequence turnoff](../../../../main-sequence-turnoff.md), with uncertainties from distances, composition and input stellar physics. A pre-examination [globular-cluster age constraint on cosmology](../../../../globular-cluster-age-constraint-on-cosmology.md) obtained a $95\%$ lower cosmic-age limit of $11\ \mathrm{Gyr}$ after allowing for formation time. This conflicts with the $9.05\ \mathrm{Gyr}$ model but is compatible with the $13.09\ \mathrm{Gyr}$ calculation.[Abstract and stellar-age/formation-time analysis](../../../../new-globular-cluster-age-estimates-and-constraints-on-the-cosmic-equation-of-state-and-the-matter-density-of-the-universe-by-lawrence-m-krauss-and-brian-chaboyer.md) Individual [stellar age](../../../../stellar-age.md) estimates are not exact clocks, and the numerical $13.09\ \mathrm{Gyr}$ is the result for the specified $H_0$ and matter fraction, not a claim to be a contemporary best-fit age.

**Constant nonzero [pressure](../../../../pressure-split.md) parameter.** Eliminating $\rho$ before setting the [pressure](../../../../pressure-split.md) to zero instead gives

$$
\begin{aligned}
\dot H
&=\frac{\Lambda}{3}-H^2-\frac{1+\epsilon}{2}
\left(H^2-\frac{\Lambda}{3}\right)\\
&=-\frac{3+\epsilon}{2}
\left(H^2-\frac{\Lambda}{3}\right).
\end{aligned}
$$

Hence

$$
\boxed{\frac{2}{3+\epsilon}\dot H+H^2-\frac{\Lambda}{3}=0}.
$$

For constant $\epsilon>-3$, the positive-density expanding Big-Bang branch is

$$
\boxed{H(t)=H_\Lambda\coth\left(\frac{3+\epsilon}{2}H_\Lambda t\right),
\qquad H_\Lambda=\sqrt{\frac{\Lambda}{3}}}.
$$

Equivalently use $t'=(3+\epsilon)t/3$ in the [pressureless matter](../../../../pressureless-matter.md) solution. The [scale factor](../../../../scale-factor-cosmology.md) obeys $R\propto\sinh^{2/(3+\epsilon)}[(3+\epsilon)H_\Lambda t/2]$, and the early limit is $H\simeq2/[(3+\epsilon)t]$. The [age of a flat barotropic matter-vacuum universe](../../../../age-of-a-flat-barotropic-matter-vacuum-universe.md) with the same present [density](../../../../density.md) fractions and $H_0$ is

$$
t_0(\epsilon)=\frac{2\,\operatorname{artanh}\sqrt{\Omega_{\Lambda0}}}
{(3+\epsilon)H_0\sqrt{\Omega_{\Lambda0}}}
=\frac{3}{3+\epsilon}t_0(0).
$$

Thus

$$
\boxed{t_0(0.2)\simeq12.28\ \mathrm{Gyr}.}
$$

The small positive [pressure](../../../../pressure-split.md) makes the early universe expand with a smaller age at the same late expansion parameters.

**The acceleration transition.** Normalize the present [scale factor](../../../../scale-factor-cosmology.md) to one. Constant $\epsilon$ and the continuity equation give $\rho=\rho_0(1+z)^{3+\epsilon}$. Dividing the acceleration equation by $H_0^2$ gives

$$
\frac{\ddot R}{R H_0^2}
=\Omega_{\Lambda0}-\frac{1+\epsilon}{2}
\Omega_{m0}(1+z)^{3+\epsilon}.
$$

At the [barotropic matter-vacuum acceleration transition](../../../../barotropic-matter-vacuum-acceleration-transition.md) its right-hand side vanishes. For the parameters here, $1+\epsilon>0$, so the past transition is

$$
\boxed{z_{\rm tr}=
\left[\frac{2(1-\Omega_{m0})}{(1+\epsilon)\Omega_{m0}}\right]^{1/(3+\epsilon)}-1
\simeq0.529}.
$$

At greater [redshift](../../../../redshift.md) the material term dominates and expansion decelerates; at smaller [redshift](../../../../redshift.md) vacuum [energy](../../../../energy-split.md) dominates and expansion accelerates. The [pressure](../../../../pressure-split.md) factor $1+\epsilon$ belongs in the numerator of the gravitating material term; omitting it would confuse this model with [pressureless matter](../../../../pressureless-matter.md).

<a id="2/image-original-constant-pressure-parameter-expansion-histories-and-acceleration-transitions"></a>
![](../../../../past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2015/paper-1-cosmic-expansion.png)

**[Figure 2](#2/image-original-constant-pressure-parameter-expansion-histories-and-acceleration-transitions). Original constant-pressure-parameter expansion histories and acceleration transitions**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
