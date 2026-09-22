<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\theta=i\mathbf k\cdot\mathbf v$. The [synchronous perfect-fluid density equation](../../../../../../synchronous-perfect-fluid-density-equation.md) and [Cosmological Euler equation in synchronous gauge](../../../../../../cosmological-euler-equation-in-synchronous-gauge.md) give

$$
\delta'=-(1+w)(\theta+h'/2),\qquad\theta'+(1-3w)\mathcal H\theta-\frac{w}{1+w}k^2\delta=0.
$$

Differentiate the first equation and use the second and the scalar trace metric equation. Before making a nonrelativistic approximation, the result is

$$
\delta''+\mathcal H\delta'+\left[wk^2-\frac32(1+w)(1+3w)\mathcal H^2\right]\delta=-3w(1+w)\mathcal H\theta.
$$

For $w=w_m=c_s^2\ll1$, discard relative pressure corrections to the background gravitational and damping terms, while retaining $c_s^2k^2$ because a large wavenumber can compensate a small sound speed. Matter domination and the flat [Friedmann equation](../../../../../../friedmann-equations.md) give $\tfrac32\mathcal H^2=4\pi G\bar\rho_m a^2$. Thus the leading [nonrelativistic density equation in synchronous gauge](../../../../../../nonrelativistic-density-equation-in-synchronous-gauge.md) is

$$
\boxed{\delta_m''+\mathcal H\delta_m'+(c_s^2k^2-4\pi G\bar\rho_m a^2)\delta_m\simeq0.}
$$

The approximation sign records the small finite-$w$ terms just displayed; the printed Newtonian-form equation is not an exact relativistic equation at nonzero $w$.

The comoving [Jeans wavenumber](../../../../../../jeans-wavenumber.md) balances pressure and gravity: $c_s^2k_J^2=4\pi G\bar\rho_m a^2$. Defining physical wavelength as $2\pi a/k$, the physical [Jeans length](../../../../../../jeans-length.md) is

$$
\boxed{\lambda_J=\frac{2\pi a}{k_J}=c_s\sqrt{\frac\pi{G\bar\rho_m}}.}
$$

For wavelengths longer than this scale, gravity can overcome pressure and density modes grow; shorter modes are pressure-supported acoustic oscillations, with expansion modifying both growth and damping. Before [cosmological recombination](../../../../../../recombination-cosmology.md), the tightly coupled [photon-baryon fluid](../../../../../../photon-baryon-fluid.md) has substantial photon pressure, $c_{s,\gamma b}^2=1/[3(1+R_b)]$, where $R_b=3\bar\rho_b/(4\bar\rho_\gamma)$. The baryonic Jeans scale is correspondingly large, so baryons oscillate instead of freely collapsing on small scales. [Cold dark matter](../../../../../../cold-dark-matter.md) has a much smaller pressure scale and can supply gravitational potential wells. After [photon decoupling](../../../../../../photon-decoupling.md), baryons lose photon pressure support and their sound speed falls to its thermal-gas value; the [baryon Jeans length across recombination](../../../../../../baryon-jeans-length-across-recombination.md) drops, allowing baryons to fall into those wells. The earlier photon-coupled fluid is not itself a constant-small-$w$ fluid; its role is a physical comparison of pressure support, not an extension of the preceding approximation through recombination.

Define a normalized smoothing window on physical radius $R$, with comoving radius $r=R/a$. If $\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle=(2\pi)^3\delta_D(\mathbf k-\mathbf k')P(k,\tau)$, the [smoothed matter density variance](../../../../../../smoothed-matter-density-variance.md) is

$$
\sigma_R^2(\tau)=\langle\delta_R^2\rangle=\frac1{2\pi^2}\int_0^\infty k^2P(k,\tau)|W(kr)|^2dk.
$$

Thus $\sigma_R$ is the root-mean-square amplitude. For a Gaussian window, $W(u)=e^{-u^2/2}$; this choice makes the scale-free integral ultraviolet convergent.

On scales where pressure is negligible, a flat matter-dominated universe has $a\propto\tau^2$, $\mathcal H=2/\tau$, and $4\pi G\bar\rho_m a^2=6/\tau^2$. The density equation has powers satisfying $s(s-1)+2s-6=0$, so

$$
\delta_m=C_+\tau^2+C_-\tau^{-3}.
$$

Select the growing mode and exclude residual synchronous gauge modes. Starting with $P(k,\tau_{\rm eq})=Ak$ gives $P(k,\tau)=Ak(\tau/\tau_{\rm eq})^4$. The [dimensionless cosmological power spectrum](../../../../../../dimensionless-cosmological-power-spectrum.md) is then

$$
\mathcal P_\delta(k,\tau)=\frac{k^3P(k,\tau)}{2\pi^2}=\frac{A}{2\pi^2\tau_{\rm eq}^4}(k\tau)^4.
$$

At [cosmological horizon crossing](../../../../../../cosmological-horizon-crossing.md), $k\sim aH=\mathcal H$, hence $k\tau\sim2$, and

$$
\boxed{\mathcal P_\delta(k,\tau_H)=\frac{8A}{\pi^2\tau_{\rm eq}^4},\qquad\text{independent of }k.}
$$

For the smoothed [variance](../../../../../../variance-split.md), change variables to $u=kr$:

$$
\sigma_R^2=\frac{A}{2\pi^2r^4}\left(\frac\tau{\tau_{\rm eq}}\right)^4\int_0^\infty u^3|W(u)|^2du.
$$

The Gaussian integral equals $1/2$. At a physical Hubble-radius window, $R=H^{-1}$ and $r=\tau/2$, giving the [Gaussian horizon-crossing variance for a Harrison-Zeldovich spectrum](../../../../../../gaussian-horizon-crossing-variance-for-a-harrison-zeldovich-spectrum.md)

$$
\boxed{\sigma_{H^{-1}}^2=\frac{4A}{\pi^2\tau_{\rm eq}^4},\qquad\text{constant at crossing}.}
$$

The window-dependent numerical constant is secondary; cancellation of the scale dependence is the [Harrison-Zeldovich spectrum](../../../../../../harrison-peebles-zeldovich-spectrum.md) property. This demonstration uses the growing pressureless matter-era idealization and therefore applies to modes crossing in that era. Modes which crossed before equality require radiation-era transfer and cannot be evolved through that period with the matter equation. A pure $P\propto k$ spectrum with a real-space top-hat window also has a logarithmically divergent ultraviolet [variance](../../../../../../variance-split.md) unless a physical high-$k$ cutoff or transfer function is supplied; the Gaussian choice makes the stated idealized [variance](../../../../../../variance-split.md) well defined.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
