<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a stationary, non-streaming tracer population with [spherical symmetry](../../../../../spherical-symmetry.md) in its full velocity distribution. In particular, the mean velocities vanish, the mixed [covariances](../../../../../covariance.md) vanish, and the two tangential components have equal [velocity dispersions](../../../../../velocity-dispersion.md). Write

$$
\sigma_r^2=\sigma_{rr}^2,\qquad
\sigma_t^2=\sigma_{\theta\theta}^2=\sigma_{\phi\phi}^2,\qquad
\beta(r)=1-\frac{\sigma_t^2}{\sigma_r^2}.
$$

Here $\sigma_t^2$ is the variance of one tangential component. In the alternative convention using the sum of both tangential variances, the same [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) is $1-(\sigma_\theta^2+\sigma_\phi^2)/(2\sigma_r^2)$. These definitions agree; they must not be mixed by inserting an extra factor of two.

The time derivative and mean-velocity terms in the supplied [Jeans equation](../../../../../jeans-equation.md) vanish, as do its angular mixed-moment terms. Its remaining geometric term is $2\nu(\sigma_r^2-\sigma_t^2)/r$. Thus the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md) becomes

$$
\boxed{\frac{d(\nu\sigma_r^2)}{dr}+\frac{2\beta(r)}r\nu\sigma_r^2
=-\nu\frac{d\Phi}{dr}.}
$$

The no-streaming assumption excludes a steady radial flow; stationarity of the density alone would not remove its advective terms.

By the [shell theorem](../../../../../spherical-shell-theorem.md), the [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) of a spherical mass distribution satisfies $d\Phi/dr=GM(<r)/r^2$. Expanding the derivative above, dividing by $\nu$, and using [logarithmic derivatives](../../../../../logarithmic-derivative.md) gives

$$
\boxed{M(<r)=-\frac{r\sigma_r^2}{G}
\left[\frac{d\ln\nu}{d\ln r}+\frac{d\ln\sigma_r^2}{d\ln r}+2\beta(r)\right].}
$$

The tracer density $\nu$ need not be the density of the gravitating matter. The [circular speed](../../../../../circular-speed.md) is $V_c^2=r\,d\Phi/dr=GM(<r)/r$, whether or not the tracers themselves follow circular orbits.

Now let $\beta$ be constant, $\nu=\nu_0(r/r_0)^{-\gamma}$, and $V_c^2=V_0^2(r/r_0)^{2\alpha}$. With $y=\sigma_r^2$, the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md) reads

$$
y'+\frac{2\beta-\gamma}{r}y=-\frac{V_c^2(r)}r.
$$

For a [power-law ansatz](../../../../../power-law-ansatz.md) $y=K V_c^2$, $y'=2\alpha y/r$, so $(\gamma-2\beta-2\alpha)y=V_c^2$. Therefore the [scale-free spherical Jeans solution](../../../../../scale-free-spherical-jeans-solution.md) is

$$
\boxed{\sigma_r^2(r)=\frac{V_c^2(r)}{\gamma-2\beta-2\alpha},\qquad
\gamma-2\beta-2\alpha>0.}
$$

The positivity condition is necessary for this particular solution to be a physical [velocity dispersion](../../../../../velocity-dispersion.md).

There is a boundary condition implicit in selecting this solution. The [integrating factor](../../../../../integrating-factor.md) $r^{2\beta-\gamma}$ gives, when $D=\gamma-2\beta-2\alpha\ne0$,

$$
y(r)=\frac{V_c^2(r)}D+C\left(\frac r{r_0}\right)^{\gamma-2\beta}.
$$

The homogeneous term represents an additional radial-pressure boundary contribution. It is removed, for example, by requiring $r^{2\beta}\nu\sigma_r^2\to0$ at infinity. Under that condition,

$$
\sigma_r^2(r)=\frac{r^{-2\beta}}{\nu(r)}
\int_r^\infty\nu(s)V_c^2(s)s^{2\beta}\frac{ds}{s},
$$

and convergence requires $D>0$, giving the boxed result. If $D=0$, the solution instead has the logarithmic form

$$
y(r)=\left(\frac r{r_0}\right)^{2\alpha}
\left[C-V_0^2\ln\frac r{r_0}\right],
$$

so the quoted constant proportionality does not apply. A finite outer boundary can retain a homogeneous term even when $D\ne0$.

To derive the [heliocentric projection of a spherical velocity dispersion](../../../../../heliocentric-projection-of-a-spherical-velocity-dispersion.md), put the Sun at vector $\boldsymbol R_\odot$ of length $R_\odot$, and a tracer at $\boldsymbol r=r\hat{\boldsymbol r}$. Its heliocentric [line of sight](../../../../../line-of-sight.md) is

$$
\hat{\boldsymbol\ell}=\frac{\boldsymbol r-\boldsymbol R_\odot}{d},\qquad
d^2=r^2+R_\odot^2-2rR_\odot u,
\qquad u=\hat{\boldsymbol r}\cdot\hat{\boldsymbol R}_\odot.
$$

If $\chi$ is the angle between $\hat{\boldsymbol\ell}$ and the Galactocentric radial direction, then

$$
\cos\chi=\frac{r-R_\odot u}{d},\qquad
\sin^2\chi=\frac{R_\odot^2(1-u^2)}{r^2+R_\odot^2-2rR_\odot u}.
$$

After correction for the Sun's motion, the intrinsic [covariance matrix](../../../../../covariance-matrix.md) has eigenvalues $\sigma_r^2,\sigma_t^2,\sigma_t^2$ in the local spherical basis. Projection onto the [line of sight](../../../../../line-of-sight.md) therefore gives

$$
\sigma_{\rm los}^2(r,u)=\sigma_r^2\cos^2\chi+\sigma_t^2\sin^2\chi
=\sigma_r^2(r)\left[1-\beta(r)\sin^2\chi\right].
$$

At fixed $r$, $\sigma_r$ and $\beta$ are constant across the spherical shell. Averaging its squared [line of sight](../../../../../line-of-sight.md) velocity, with zero mean, gives

$$
\boxed{\sigma_\odot(r)=\sigma_r(r)\sqrt{1-\beta(r)A(r,R_\odot)},\qquad
A=\langle\sin^2\chi\rangle.}
$$

For a uniformly sampled Galactocentric shell, the [solid angle](../../../../../solid-angle.md) measure makes $u$ uniform on $[-1,1]$, giving the [geometric correction for heliocentric velocity dispersion](../../../../../geometric-correction-for-heliocentric-velocity-dispersion.md)

$$
A(r,R_\odot)=\frac{R_\odot^2}{2}
\int_{-1}^1\frac{1-u^2}{r^2+R_\odot^2-2rR_\odot u}\,du.
$$

To evaluate it, set $a=r^2+R_\odot^2$ and $b=2rR_\odot$, and divide the integrand:

$$
\frac{1-u^2}{a-bu}=\frac{u}{b}+\frac{a}{b^2}
+\frac{1-a^2/b^2}{a-bu}.
$$

The odd term integrates to zero, while $\int_{-1}^1du/(a-bu)=b^{-1}\ln[(a+b)/(a-b)]$. For $r>0$, $R_\odot>0$, and $r\ne R_\odot$, this gives

$$
\boxed{A(r,R_\odot)=\frac{r^2+R_\odot^2}{4r^2}
-\frac{(r^2-R_\odot^2)^2}{8r^3R_\odot}
\ln\left|\frac{r+R_\odot}{r-R_\odot}\right|.}
$$

The removable limit at $r=R_\odot$ is $A=1/2$. As $r/R_\odot\to\infty$, $A\simeq2R_\odot^2/(3r^2)$, while as $r/R_\odot\to0$, $A\to2/3$. If $R_\odot=0$, $A=0$ and the observed [velocity dispersion](../../../../../velocity-dispersion.md) is exactly radial. For isotropic velocities, $\beta=0$, the correction vanishes at every radius.

The averaging measure matters. If directions are instead uniform in heliocentric [solid angle](../../../../../solid-angle.md) at a fixed Galactocentric radius $r>R_\odot$, let $\vartheta$ be the angle between the [line of sight](../../../../../line-of-sight.md) and $\boldsymbol R_\odot$. Geometry gives $\sin^2\chi=(R_\odot/r)^2\sin^2\vartheta$, so that particular weighting gives $A=2R_\odot^2/(3r^2)$ exactly. The logarithmic expression above uses uniform tracer weighting on a Galactocentric shell. For an observational sample, use its actual angular selection weights in $A=\langle\sin^2\chi\rangle$; the boxed dispersion relation remains valid.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
