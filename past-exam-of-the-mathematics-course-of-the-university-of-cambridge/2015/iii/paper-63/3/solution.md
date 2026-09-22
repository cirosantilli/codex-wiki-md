<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $R_p$ for the physical planet radius and $R_c=\eta R_{H1}$ for the debris-cloud radius; the source uses $R_1$ for both even though their stated size orderings are opposite. A central [transit duration of a small planet](../../../../../transit-duration-of-a-small-planet.md) on a nearly circular [Kepler orbit](../../../../../kepler-orbit.md) is $D_p\simeq2R_\star/(n_1a_1)=P_1R_\star/(\pi a_1)$. [Kepler's third law](../../../../../kepler-s-third-law.md), with $M_\star=4\pi\rho_\star R_\star^3/3$, gives

$$
\frac{P_1}{D_p^3}\simeq\frac{\pi^2G\rho_\star}{3}.
$$

A noncentral planetary [exoplanet transit](../../../../../exoplanet-transit.md) is shorter, so within the small-radius and nearly circular approximations, a duration requiring

$$
\boxed{\frac{P_1}{D_1^3}<\frac{\pi^2G\rho_\star}{3}}
$$

is too long for the planet alone and favors extended debris. For a central cloud transit with $R_c\gg R_\star$, the path length is approximately $2R_c$. Using the [Hill radius](../../../../../hill-radius.md) $R_{H1}=a_1(M_1/(3M_\star))^{1/3}$ gives $D_1/P_1\simeq R_c/(\pi a_1)$, hence the [Hill-cloud transit mass estimate](../../../../../hill-cloud-transit-mass-estimate.md)

$$
\boxed{\frac{M_1}{M_\star}\simeq3\left(\frac{\pi D_1}{\eta P_1}\right)^3.}
$$

This equality assumes a central cloud chord. An orbit described merely as nearly edge-on need not have central cloud crossings. If its projected cloud impact distance is $s$, the measured half-chord is $\sqrt{R_c^2-s^2}$, so the boxed mass is multiplied by $[1-(s/R_c)^2]^{-3/2}$. It is a lower estimate when that geometry is unknown.

For the dynamical calculation use $\mu_2=M_2/M_\star$, $A=GM_2/a_2$, and $\mathcal R=A f(\alpha)e_1\cos\phi_1$. The derivatives in the supplied [Lagrange planetary equations](../../../../../lagrange-planetary-equations.md) hold the other [osculating orbital elements](../../../../../osculating-orbital-element.md) fixed:

$$
\partial_{\lambda_1}\mathcal R=jAf e_1\sin\phi_1,
\quad \partial_{a_1}\mathcal R=\frac A{a_2}f'e_1\cos\phi_1,
\quad \partial_{e_1}\mathcal R=Af\cos\phi_1.
$$

Since $A/(n_1a_1^2)=n_1\mu_2\alpha$, the physical [mean-longitude equation for a first-order resonant term](../../../../../mean-longitude-equation-for-a-first-order-resonant-term.md) is

$$
\boxed{\dot\lambda_1=n_1[1+\mu_2g(\alpha)e_1\cos\phi_1],\qquad
 g(\alpha)=\frac\alpha2f(\alpha)-2\alpha^2f'(\alpha).}
$$

The source's epoch notation needs care when $n_1$ varies. Literally differentiating $\lambda_1=n_1(t)t+\epsilon_1(t)$ adds $t\dot n_1$; one cannot retain that definition and also identify the printed $\dot\epsilon_1$ with $\dot\lambda_1-n_1$. A consistent version writes $\lambda_1=\int_0^t n_1(s)\,ds+\epsilon_{\rm int}$ and assigns the displayed correction to $\dot\epsilon_{\rm int}$. Equivalently, the canonical [mean-longitude equation for a first-order resonant term](../../../../../mean-longitude-equation-for-a-first-order-resonant-term.md) follows from the [disturbing function](../../../../../disturbing-function.md) directly. The result for $g$ is the intended physical equation under that convention.

Away from [resonant-argument libration](../../../../../resonant-argument-libration.md), neglect changes in $e_1,\alpha,\varpi_1$ on one slow cycle to this order. With $n_0=2\pi/P_1$ the reference [mean motion](../../../../../mean-motion.md), the signed slow frequency is

$$
\omega=(j+1)n_2-jn_0=-\frac{jn_0\Delta}{1+\Delta},\qquad
P_t=\frac{2\pi}{|\omega|}=\frac{P_1(1+\Delta)}{j|\Delta|}.
$$

This is the [near-resonant transit-timing superperiod](../../../../../near-resonant-transit-timing-superperiod.md). Choose $\phi_1(0)=0$. Differentiating $n_1\propto a_1^{-3/2}$ with the [semi-major axis](../../../../../semi-major-axis.md) equation gives

$$
\dot n_1=-3j\mu_2n_0^2\alpha f e_1\sin(\omega t).
$$

Let $C=3j\mu_2n_0^2\alpha f e_1$ and $n_s=n_1(0)$. Direct [integration](../../../../../integral.md) gives

$$
n_1(t)=n_s+\frac C\omega[\cos(\omega t)-1],
\qquad
\lambda_1(t)=\left(n_s-\frac C\omega\right)t
+\left(\frac C{\omega^2}+\frac{n_0\mu_2g e_1}{\omega}\right)\sin(\omega t),
$$

with zero initial [mean longitude](../../../../../mean-longitude.md). The constant and linear terms are absorbed into the fitted transit ephemeris: the measured mean frequency is $\bar n=n_s-C/\omega$. This distinction avoids mistaking an arbitrary initial frequency for the long-term fitted period.

For $|\Delta|\ll1$, the double-integrated frequency term dominates the direct $g$ term provided $g/f$ stays finite. Relative to the fitted linear ephemeris, $\lambda_1(t_k)=2\pi k$ gives

$$
t_k\simeq P_1k+A_t\sin(\omega t_k),\qquad
A_t=-\frac{3j\mu_2n_0\alpha f e_1}{\omega^2}
\simeq-\frac{3\mu_2\alpha f e_1}{jn_0\Delta^2}.
$$

Here $P_1$ denotes the fitted mean period at the retained order. The signed-frequency convention fixes the phase sign. Replacing $\omega$ by $2\pi/P_t>0$ changes the sign of the signed $A_t$ when needed; a nonnegative amplitude has

$$
\boxed{\frac{|A_t|}{P_t}\simeq\frac3{2\pi}\mu_2\frac{\alpha|f(\alpha)|e_1}{|\Delta|}.}
$$

Using a signed $P_t=2\pi/\omega$ instead gives the source's signed proportionality $A_t/P_t\simeq3\mu_2\alpha f e_1/(2\pi\Delta)$. The leading implicit transit equation can equally use $P_1k$ inside the sine, since the difference is higher order in the perturbation. This is the [eccentricity-enhanced near-resonant transit-timing variation](../../../../../eccentricity-enhanced-near-resonant-transit-timing-variation.md); its derivation assumes small longitude oscillations, $\mu_2e_1\ll\Delta^2$ at fixed resonance coefficients, and the effectively fixed eccentricity used in this truncated model. Dominance over forced-eccentricity timing terms typically also requires $e_1\gg|\Delta|$ at fixed $j$. A full transit calculation also includes forced [orbital eccentricity](../../../../../orbital-eccentricity.md) and the conversion from [mean longitude](../../../../../mean-longitude.md) to the actual sky-crossing angle. Those are lower order in this eccentricity-enhanced regime, rather than identically absent; broader near-resonant formulas are derived by [Lithwick, Xie and Wu](https://arxiv.org/abs/1207.4192).

Inside a [mean-motion resonance](../../../../../mean-motion-resonance.md), $\phi_1$ undergoes [resonant-argument libration](../../../../../resonant-argument-libration.md) and its evolution must be solved together with $a_1,e_1,\varpi_1$. The constant circulation frequency $\omega$ and the associated $\Delta^{-2}$ expansion then fail. At approximately fixed eccentricity, the resonant [resonant pendulum approximation](../../../../../pendulum-approximation-of-a-mean-motion-resonance.md) has libration frequency of order $jn_0\sqrt{\mu_2\alpha|f|e_1}$, up to numerical factors. The [transit-timing variation](../../../../../transit-timing-variation.md) follows that libration period and depends on its [libration amplitude of a resonant argument](../../../../../libration-amplitude-of-a-resonant-argument.md). Exactly at a resonant equilibrium there need be no libration signal; near a [separatrix](../../../../../separatrix.md) the period grows, and eccentricity dynamics can modify the simple estimate. Resonant amplitudes remain controlled by the bounded resonant motion rather than diverging as the circulating detuning tends to zero.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
