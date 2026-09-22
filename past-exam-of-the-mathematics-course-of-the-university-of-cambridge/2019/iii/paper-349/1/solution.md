<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $Q=\dot N_{\rm ion}$ for the constant [hydrogen-ionizing photon production rate](../../../../../hydrogen-ionizing-photon-production-rate.md). Assume an initially neutral gas of [hydrogen atoms](../../../../../hydrogen-atom.md), a sharp spherical [ionization front](../../../../../ionization-front.md), complete ionization inside it, and a fixed gas density. The [Electron](../../../../../electron.md) and [proton](../../../../../proton.md) number densities inside are then both $n$. Take the recombination coefficient $\alpha$ to be constant, with the usual [Case B recombination](../../../../../case-b-recombination.md) interpretation: photons from recombination directly to the ground state are absorbed locally. Neglect absorption by dust, pressure-driven gas motion, and light-travel delays.

The total rate of [Case B recombination](../../../../../case-b-recombination.md) within radius $R$ is

$$
\mathcal R(R)=\int_0^R\alpha n_e n_p\,4\pi r^2\,dr
=\frac{4\pi}{3}\alpha n^2R^3.
$$

At [photoionization equilibrium](../../../../../photoionization-equilibrium.md), $Q=\mathcal R(R_S)$, giving the [Strömgren radius](../../../../../stromgren-radius.md)

$$
\boxed{R_S=\left(\frac{3Q}{4\pi\alpha n^2}\right)^{1/3}.}
$$

The square of the density appears because recombination requires encounters between an [Electron](../../../../../electron.md) and a [proton](../../../../../proton.md).

During [Ionization-front growth of a Strömgren sphere](../../../../../ionization-front-growth-of-a-stromgren-sphere.md), each photon either replaces an ion lost through [Case B recombination](../../../../../case-b-recombination.md) or ionizes an additional atom. There are $N_i=(4\pi/3)nR^3$ ions inside the [ionization front](../../../../../ionization-front.md), so photon counting gives

$$
\frac{dN_i}{dt}=Q-\alpha nN_i,
\qquad
4\pi nR^2\frac{dR}{dt}=Q-\frac{4\pi}{3}\alpha n^2R^3.
$$

The [recombination time](../../../../../recombination-time.md) is $t_{\rm rec}=(\alpha n)^{-1}$. Solving this first-order [differential equation](../../../../../differential-equation-split.md) with $R(0)=0$ gives

$$
N_i(t)=Qt_{\rm rec}\left(1-e^{-t/t_{\rm rec}}\right),\qquad
\boxed{\frac{R(t)}{R_S}=\left(1-e^{-t/t_{\rm rec}}\right)^{1/3}.}
$$

For an initial radius $R_0$, the corresponding result is $R^3(t)=R_S^3+(R_0^3-R_S^3)e^{-t/t_{\rm rec}}$. Initially, the idealized photon-counting solution has $R\simeq[3Qt/(4\pi n)]^{1/3}$; at late times, $R/R_S\simeq1-\tfrac13e^{-t/t_{\rm rec}}$. The initially divergent front speed in this approximation is a consequence of neglecting light-travel delays; the formula describes the growth once that approximation is applicable.

For a [power law](../../../../../power-law.md) density, specify a reference radius $r_0$ so that $n(r)=n_0(r/r_0)^{-\beta}$. With an inner cutoff $r_{\rm in}>0$, the [recombination integral for a power-law nebula](../../../../../recombination-integral-for-a-power-law-nebula.md) is

$$
\mathcal R(R;r_{\rm in})=4\pi\alpha n_0^2r_0^{2\beta}
\begin{cases}
\displaystyle\frac{R^{3-2\beta}-r_{\rm in}^{3-2\beta}}{3-2\beta},&\beta\ne\frac32,\\[6pt]
\displaystyle\ln\frac{R}{r_{\rm in}},&\beta=\frac32.
\end{cases}
$$

Equivalently, a logarithmic interval in radius contributes $d\mathcal R/d\ln r=4\pi\alpha n_0^2r_0^{2\beta}r^{3-2\beta}$. For $\beta<3/2$, the central integral converges as $r_{\rm in}\to0$, and the recombination rate grows as $R^{3-2\beta}$. At $\beta=3/2$, each logarithmic interval contributes equally and the centre gives a logarithmic divergence. For $\beta>3/2$, the unmodified profile gives a power divergence at the centre, while its outer recombination integral converges. The change at $\beta=3/2$ is set by the competition between the spherical volume element and the squared density.

To regularize the centre, choose the following explicit [cored power-law density profile](../../../../../cored-power-law-density-profile.md), taking $r_0=r_c$ and $n_0$ as the core density:

$$
n(r)=\begin{cases}
n_0,&0\leq r\leq r_c,\\
n_0(r/r_c)^{-\beta},&r>r_c.
\end{cases}
$$

For $R\leq r_c$, $\mathcal R(R)=(4\pi/3)\alpha n_0^2R^3$. For $R>r_c$, put $u=R/r_c$ and integrate the core and envelope separately:

$$
\mathcal R(R)=4\pi\alpha n_0^2r_c^3
\begin{cases}
\displaystyle\frac13+\frac{u^{3-2\beta}-1}{3-2\beta},&\beta\ne\frac32,\\[6pt]
\displaystyle\frac13+\ln u,&\beta=\frac32.
\end{cases}
$$

This rate is continuous and strictly increasing with $R$. If $\beta>3/2$, it has a finite supremum, the [critical ionizing photon rate of a cored power-law nebula](../../../../../critical-ionizing-photon-rate-of-a-cored-power-law-nebula.md):

$$
\boxed{Q_{\rm crit}=4\pi\alpha n_0^2r_c^3
\left(\frac13+\frac1{2\beta-3}\right)
=\frac{8\pi\alpha\beta n_0^2r_c^3}{3(2\beta-3)}.}
$$

For $0<Q<Q_{\rm crit}$ there is a unique finite radius at [photoionization equilibrium](../../../../../photoionization-equilibrium.md). At $Q=Q_{\rm crit}$ the equality is approached only as $R\to\infty$; for $Q>Q_{\rm crit}$ even ionizing the whole profile cannot consume all photons through [Case B recombination](../../../../../case-b-recombination.md), so no equilibrium radius exists. For $\beta\leq3/2$, the envelope integral grows without bound and there is no finite critical rate in this infinite-extent model.

For a concrete choice, take any $n_0>0$, $r_c>0$, and $\beta=2$. Then $Q_{\rm crit}=16\pi\alpha n_0^2r_c^3/3$. In the envelope, defining $q=Q/(4\pi\alpha n_0^2r_c^3)$ gives $R=r_c/(4/3-q)$ for $1/3<q<4/3$, explicitly showing the divergence as the critical rate is approached. A different core shape changes the numerical coefficient of $Q_{\rm crit}$, while the outer-slope condition $\beta>3/2$ remains the same.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
