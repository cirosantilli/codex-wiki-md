<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

There is a genuine inconsistency in this part. For any nonnegative [metallicity distribution function](../../../../../metallicity-distribution-function.md), its maximum is at least its mean. A population of positive mean solar [metallicity](../../../../../metallicity.md) cannot have a maximum equal to half that mean. For example, a uniform abundance distribution on $[0,2Z_\odot]$ has mean $Z_\odot$ and maximum $2Z_\odot$. Thus the printed maximum-to-mean ratio cannot be proved. The following calculation explains the supplied function, gives the consistent distribution, and also treats the literal birth-metallicity interpretation separately.

Let $f(\mu)$ denote the supplied abundance function. Algebraically it is

$$
f(\mu)=\frac{Y-(Y+1)\mu+\mu^{Y+1}}{(Y+1)(1-\mu)}.
$$

With $\delta=1-\mu$, a [Taylor series](../../../../../taylor-series.md) of $(1-\delta)^{Y+1}$ gives

$$
f(1-\delta)=\frac{Y\delta}{2}+\frac{Y(1-Y)\delta^2}{6}+O(\delta^3).
$$

Consequently

$$
\boxed{f(1-\delta)\simeq\frac{Y\delta}{2}.}
$$

This is an early-consumption expansion: its fractional correction is $(1-Y)\delta/3+O(\delta^2)$. Small yield alone does not make the expression linear throughout most of the gas-consumption history. At fixed $0<\mu<1$, the small-$Y$ expansion instead is

$$
f(\mu)=Y\left[1+\frac{\mu\log\mu}{1-\mu}\right]+O(Y^2).
$$

In a well-mixed [closed-box model of galactic chemical evolution](../../../../../closed-box-model-of-galactic-chemical-evolution.md), the [gas fraction of a galaxy](../../../../../gas-fraction-of-a-galaxy.md) also labels the permanently locked stellar mass: $dM_s=-M_{g,\rm init}\,d\mu$. Newly formed stars inherit the current [gas-phase metallicity](../../../../../gas-phase-metallicity.md) $Z_g(\mu)$. Therefore the mass-weighted mean [stellar metallicity](../../../../../stellar-metallicity.md) satisfies the [cumulative and birth stellar metallicities](../../../../../cumulative-and-birth-stellar-metallicities.md) relation

$$
\overline Z_*(\mu)=\frac1{1-\mu}\int_\mu^1 Z_g(u)\,du,\qquad
Z_g(\mu)=-\frac{d}{d\mu}[(1-\mu)\overline Z_*(\mu)].
$$

Applying the derivative to $f$ gives

$$
\boxed{\overline Z_*(\mu)=f(\mu)\quad\Longleftrightarrow\quad Z_{\rm birth}(\mu)=Z_g(\mu)=1-\mu^Y.}
$$

Thus the supplied function has the natural interpretation of a cumulative mean, not an individual star's birth abundance. Direct integration of $1-u^Y$ verifies that it gives exactly $f$. This is the [saturating closed-box enrichment law](../../../../../saturating-closed-box-enrichment-law.md): it corresponds to effective [stellar yield](../../../../../stellar-yield.md) $Y(1-Z_g)$, with $Z_g$ measured as a fraction. The usual constant-yield trace-metal model instead gives $Z_g=-Y\log\mu$. Both agree to first order when $Y|\log\mu|\ll1$; their exact formulae should not be identified outside that regime.

Let the final gas fraction be $\mu_f>0$ and $\delta_f=1-\mu_f$. In the consistent mean-metallicity interpretation, $\overline Z_*(\mu_f)=Z_\odot$ while the most recently formed stars have the maximum $z_f=1-\mu_f^Y$. At early consumption,

$$
\overline Z_*\simeq\frac{Y\delta_f}{2},\qquad z_f\simeq Y\delta_f,
$$

so the corrected result is

$$
\boxed{Z_{*,\max}\simeq2Z_\odot.}
$$

The assumption here includes $\delta_f\ll1$, equivalently $2Z_\odot/Y\ll1$ in this approximation. Exactly, $z_f=1-\mu_f^Y$ and $Z_\odot=f(\mu_f)$ determine the maximum implicitly; it remains larger than the mean, but its ratio to the mean need not equal two after substantial consumption.

For the mass-weighted [metallicity distribution function](../../../../../metallicity-distribution-function.md), stars formed while the gas fraction falls by $-d\mu$ have probability $dP=-d\mu/\delta_f$. Writing their individual abundance as $z=1-\mu^Y$ gives $\mu=(1-z)^{1/Y}$ and the [change of variables](../../../../../change-of-variables-formula.md)

$$
\boxed{dP=F(z)\,dz,\qquad F(z)=\frac{(1-z)^{1/Y-1}}{Y(1-\mu_f)},\quad 0<z<1-\mu_f^Y.}
$$

The density is zero outside this interval. Its cumulative probability is $[1-(1-z)^{1/Y}]/(1-\mu_f)$, so it integrates to one; integrating $zF(z)$ reproduces $f(\mu_f)$. A star-count distribution has the same form if the [initial mass function](../../../../../initial-mass-function.md) and survival selection give a fixed number of observed stars per unit locked mass. Luminosity-weighted samples require different weights.

For trace abundances, $(1-z)^{1/Y-1}\simeq e^{-z/Y}$ to leading order at fixed $z/Y$. The corresponding ordinary [closed-box metallicity distribution](../../../../../closed-box-metallicity-distribution.md) is

$$
F_{\rm trace}(z)=\frac{e^{-z/Y}}{Y(1-\mu_f)},\qquad 0<z<-Y\log\mu_f.
$$

In the early-consumption regime $z_f\ll Y$, this becomes approximately uniform, $F\simeq1/(Y\delta_f)$ on $[0,Y\delta_f]$. Its mean is half its upper endpoint, again producing the corrected maximum $2Z_\odot$.

If the supplied $f(\mu)$ is instead retained literally as the individual birth abundance, set $q=f(\mu)$ rather than $z=1-\mu^Y$. The observation-time population mean is then $\delta_f^{-1}\int_{\mu_f}^1 f(u)\,du$, not $f(\mu_f)$. Its exact distribution can be specified parametrically using

$$
\frac{df}{d\delta}=\frac{1-\mu^Y-f(\mu)}{1-\mu}>0,\qquad
\boxed{F_{\rm literal}(f(\mu))=\frac{1-\mu}{(1-\mu_f)[1-\mu^Y-f(\mu)]},\quad \mu_f<\mu<1.}
$$

Positivity follows because $f$ is the average of the increasing function $1-(1-\delta)^Y$. Its support is $0<q<f(\mu_f)$, and normalization follows directly from $dP=d\delta/\delta_f$. At early consumption it is uniform with $F_{\rm literal}\simeq2/(Y\delta_f)$, maximum $Y\delta_f/2$ and mean $Y\delta_f/4$. Even this literal alternative gives maximum twice the population mean, never half. **The distinction between birth abundance and cumulative mean resolves the calculation; the printed inverse maximum-to-mean ratio is false under either interpretation.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
