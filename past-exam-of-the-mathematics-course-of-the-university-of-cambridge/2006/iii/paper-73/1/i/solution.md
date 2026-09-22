<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A local [stellar relaxation time](../../../../../../stellar-relaxation-time.md) depends on the [number density](../../../../../../number-density.md) $n$ of scatterers. Calling $N$ a total number, as the PDF does, leaves the displayed expression dimensionally wrong: $\sigma^3/(G^2m^2N)$ has units of time per volume. The intended local expression must use $n$, or $N/V$ for a homogeneous sample of [volume](../../../../../../volume.md) $V$. We shall also make the normalization of the [stellar relaxation time](../../../../../../stellar-relaxation-time.md) explicit, since an unspecified representative one-dimensional [velocity dispersion](../../../../../../velocity-dispersion.md) does not fix an exact numerical coefficient.

In a [small-angle gravitational encounter](../../../../../../small-angle-gravitational-encounter.md), approximate the relative trajectory by a straight line of [speed](../../../../../../speed.md) $u$ and [impact parameter](../../../../../../impact-parameter.md) $b$. The perpendicular acceleration of one [star](../../../../../../star.md) due to the other is $Gmb/(b^2+u^2t^2)^{3/2}$. Its impulse is therefore

$$
|\Delta v_\perp|=Gmb\int_{-\infty}^\infty\frac{dt}{(b^2+u^2t^2)^{3/2}}=\frac{2Gm}{bu}.
$$

A [star](../../../../../../star.md) encounters $2\pi b\,db\,nu$ scatterers per unit [time](../../../../../../time-in-physics.md) in this interval of [impact parameters](../../../../../../impact-parameter.md). Independent deflections have random directions, so their [variances](../../../../../../variance-split.md) add as in a [random walk](../../../../../../random-walk.md). Hence the accumulated squared [velocity](../../../../../../velocity.md) change has rate

$$
D_v\equiv\frac{d\langle|\Delta\mathbf v|^2\rangle}{dt}=\int_{b_{\min}}^{b_{\max}}\left(\frac{2Gm}{bu}\right)^2 2\pi bnu\,db=\frac{8\pi G^2m^2n}{u}\ln\Lambda,\qquad\Lambda=\frac{b_{\max}}{b_{\min}}.
$$

The [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md) arises because each logarithmic interval of [impact parameter](../../../../../../impact-parameter.md) contributes equally. The lower cutoff is approximately the strong-deflection scale, $b_{\min}\simeq G(2m)/u^2$ for equal masses, or the physical collision scale if larger. The upper cutoff is a scale on which the local density and straight-line encounter approximation cease to apply, such as the local disk thickness. Thus $\Lambda$ is dimensionless; it is not a number density or an arbitrary dimensional argument of a logarithm.

To display the normalization issue, use the representative relative [speed](../../../../../../speed.md) $u=\sqrt2\sigma$ and define $T(\kappa)$ by $D_vT=\kappa\sigma^2$. This gives

$$
T(\kappa)=\frac{\kappa}{4\pi\sqrt2}\frac{\sigma^3}{nG^2m^2\ln\Lambda}.
$$

Choosing $\kappa=3/4$ recovers precisely the printed coefficient after repairing $N$ to $n$:

$$
\boxed{T_R^{\rm printed\ convention}=\frac{3}{16\pi\sqrt2}\frac{\sigma^3}{nG^2m^2\ln\Lambda}.}
$$

This is an explicitly defined convention, not a uniquely derivable normalization from the supplied data. If instead relaxation means a mean-square change equal to the full initial random-speed variance, $3\sigma^2$, the same encounter approximation gives $T_R=4T_R^{\rm printed\ convention}$. Averaging the encounter [speed](../../../../../../speed.md) distribution instead of using one representative $u$ changes the coefficient again. The robust result is the scaling $T_R\propto\sigma^3/(nG^2m^2\ln\Lambda)$.

For a transparent solar-neighbourhood estimate, take $n=0.1\,{\rm pc}^{-3}$, $m=M_\odot$, $\sigma=30\,{\rm km\,s}^{-1}$ and $b_{\max}=300\,{\rm pc}$. With $G=4.3009\times10^{-3}\,{\rm pc}\,M_\odot^{-1}({\rm km\,s}^{-1})^2$, one obtains $b_{\min}=4.78\times10^{-6}\,{\rm pc}$, $\ln\Lambda=17.96$, and

$$
T_R^{\rm printed\ convention}\simeq3.35\times10^{13}\,{\rm yr},\qquad T_R^{\rm full\ variance}\simeq1.34\times10^{14}\,{\rm yr}.
$$

These illustrative parameters give an order $10^{13}$--$10^{14}$ year [stellar relaxation time](../../../../../../stellar-relaxation-time.md), much longer than a galactic lifetime of order $10^{10}$ years. The solar neighbourhood is consequently a [collisionless stellar system](../../../../../../collisionless-stellar-system.md) with respect to encounters between individual [stars](../../../../../../star.md). Scattering by massive clouds and collective structure is a different process; the estimate does not assert that every mechanism of disk heating is negligible.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
