<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [geometrized units](../../../../../geometrized-units.md), and denote the beacon's [proper time](../../../../../proper-time.md) by $s$ to distinguish it from the short emitted duration $\tau$. Take $s=0$ at release. The period $M$, the duration $\tau$, and the [wavelength](../../../../../wavelength.md) $\lambda$ are measured by the beacon's own clock. Its radial [timelike geodesic](../../../../../timelike-geodesic.md) has conserved [Killing energy](../../../../../killing-energy.md) per unit rest mass $E=f\,dt/ds$, where $f=1-2M/r$. Initially $dr/ds=0$ at $r=8M$, so $E=\sqrt{f(8M)}=\sqrt3/2$. Normalization of the four-velocity gives

$$
-1=-f\left(\frac{dt}{ds}\right)^2+\frac1f\left(\frac{dr}{ds}\right)^2,\qquad
\frac{dr}{ds}=-\sqrt{E^2-f}=-\sqrt{\frac{2M}{r}-\frac14}.
$$

For the [Schwarzschild radial fall from rest at a finite radius](../../../../../schwarzschild-radial-fall-from-rest-at-a-finite-radius.md), introduce

$$
r=4M(1+\cos\eta)=8M\cos^2\frac\eta2,\qquad
s=8M(\eta+\sin\eta),\qquad 0\le\eta\le\frac{2\pi}3.
$$

Indeed $ds/d\eta=8M(1+\cos\eta)$ and $dr/d\eta=-4M\sin\eta$ reproduce the inward radial equation. At the [Schwarzschild event horizon](../../../../../schwarzschild-event-horizon.md), $r=2M$ and $\cos\eta_H=-1/2$. Hence

$$
\boxed{s_H=8M\left(\frac{2\pi}3+\frac{\sqrt3}2\right)
=\left(\frac{16\pi}3+4\sqrt3\right)M\simeq23.6834M.}
$$

This is the finite falling-clock time to the [event horizon](../../../../../event-horizon.md). By contrast, [Schwarzschild time](../../../../../schwarzschild-time.md) obeys $dt/ds=E/f$ and diverges at crossing. Near the horizon $r-2M\simeq E(s_H-s)$, so $dt/ds\simeq2M/(s_H-s)$ and $t\simeq-2M\log((s_H-s)/M)+\text{constant}$.

Every outward [optical pulse](../../../../../optical-pulse.md) emitted while $r>2M$ can reach a distant observer, and no pulse emitted after entry into the future black-hole region can do so. The infinite coordinate crossing time does not produce infinite emissions, because the pulse clock runs in [proper time](../../../../../proper-time.md). If there is a pulse at release, the escape times are $s_n=nM$ for $n=0,\ldots,23$. Thus **24 pulses are received, counting the pulse at release; 23 are emitted subsequently during the fall**. More generally the PDF does not specify the phase of the pulse clock. For a first emission at $s=\delta$ with $0\le\delta<M$, the [finite pulse count for a falling Schwarzschild beacon](../../../../../finite-pulse-count-for-a-falling-schwarzschild-beacon.md) is

$$
\boxed{N(\delta)=\#\{n\ge0:\delta+nM<s_H\}
=\left\lceil\frac{s_H-\delta}{M}\right\rceil\in\{23,24\}.}
$$

The ceiling handles a pulse scheduled exactly at crossing correctly: it cannot escape. This count concerns pulses associated with the fall, not any pulses emitted before release, and assumes an ideal observer able to detect arbitrarily redshifted signals.

To find the stretching of an [optical pulse](../../../../../optical-pulse.md), use the [Schwarzschild tortoise coordinate](../../../../../schwarzschild-tortoise-coordinate.md) $r_*=r+2M\log(r/(2M)-1)$. An outward [radial null geodesic](../../../../../radial-null-geodesic.md) has constant [Schwarzschild retarded null coordinate](../../../../../schwarzschild-retarded-null-coordinate.md) $u=t-r_*$. At an observer's fixed large radius $R$, its arrival time is $t_R=u+r_*(R)$; therefore only the varying emission value of $u$ contributes to the interval between arriving wavefronts. Differentiating along the falling source gives

$$
\mathcal D(r)=\frac{du}{ds}
=\frac{dt}{ds}-\frac1f\frac{dr}{ds}
=\frac{E+\sqrt{E^2-f(r)}}{f(r)}
=\frac1{E-\sqrt{E^2-f(r)}}.
$$

The [outgoing pulse redshift from a radial Schwarzschild infaller](../../../../../outgoing-pulse-redshift-from-a-radial-schwarzschild-infaller.md) includes both [gravitational redshift](../../../../../gravitational-redshift.md) and the emitter's inward [Doppler shift](../../../../../doppler-effect.md). A short pulse emitted at radius $r_e$ has, to leading order in its duration,

$$
\boxed{\tau_{\mathrm{obs}}\simeq\mathcal D(r_e)\tau,\qquad
\nu_{\mathrm{obs}}\simeq\frac1{\mathcal D(r_e)\lambda}.}
$$

For a finite receiver radius, replace $\mathcal D$ by $\sqrt{f(R)}\mathcal D$ to measure the receiver's [proper time](../../../../../proper-time.md) and [frequency](../../../../../frequency.md); this correction is negligible for $R\gg M$. The inverse scaling of [frequency](../../../../../frequency.md) follows because the number of carrier cycles is unchanged when the pulse is stretched. Here $\nu=1/\lambda$ is ordinary frequency, not angular frequency, in units with light speed one.

Under the release-phase convention, the last emission is at $s_e=23M$. Solve $8(\eta_e+\sin\eta_e)=23$ to obtain $\eta_e\simeq1.94374184$, $r_e\simeq2.54255983M$, and $\mathcal D(r_e)\simeq7.49122492$. Because $\tau\ll M$ and this pulse begins $0.683364M$ before crossing, the local short-pulse approximation applies. Thus its approximate observed duration and [frequency](../../../../../frequency.md) are

$$
\boxed{\tau_{\mathrm{last}}\simeq7.49\tau,\qquad
\nu_{\mathrm{last}}\simeq\frac{0.1335}{\lambda}\quad\text{if a pulse starts at release}.}
$$

Without fixing that phase, these numerical coefficients are not unique: put $s_e=\delta+(N(\delta)-1)M$, find $r_e$ from the parameterization, and use the boxed general formulas. For a last pulse close to crossing, with $\Delta=s_H-s_e\ll M$ but $\tau\ll\Delta$, the [horizon redshift of a Schwarzschild infaller](../../../../../horizon-redshift-of-a-schwarzschild-infaller.md) gives the useful estimates

$$
\boxed{\tau_{\mathrm{last}}\simeq\frac{4M}{\Delta}\tau,\qquad
\nu_{\mathrm{last}}\simeq\frac{\Delta}{4M\lambda}.}
$$

If a phase instead places the pulse within one pulse-duration of crossing, $\Delta\lesssim\tau$, a single constant stretching factor is inappropriate. The received extent of a complete escaping pulse is exactly $u(s_e+\tau)-u(s_e)$; a pulse straddling crossing has an escaping tail extending to arbitrarily late arrival times, whose instantaneous [frequency](../../../../../frequency.md) tends to zero. The finite count remains valid, while its last-pulse duration then has no finite constant multiple of $\tau$. This identifies precisely what the unspecified pulse phase can change.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
