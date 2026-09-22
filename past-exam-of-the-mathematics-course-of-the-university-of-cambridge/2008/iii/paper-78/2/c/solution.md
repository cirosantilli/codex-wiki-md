<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\theta(z)=\Omega\log z+\Phi$. A [fixed point](../../../../../../fixed-point.md) of the [Shilnikov return map](../../../../../../shilnikov-return-map.md) is a [periodic orbit](../../../../../../periodic-orbit.md) with one marked global excursion, and satisfies

$$
\boxed{\mu=Az^\delta\cos\theta(z)-z,\qquad
f_S'(z)=Az^{\delta-1}\bigl(\delta\cos\theta(z)-\Omega\sin\theta(z)\bigr).}
$$

Its local passage takes logarithmically long. If the global travel time tends to $T_g$, then its physical period is

$$
T=T_g+\lambda_+^{-1}\log(z_0/z)+o(1).
$$

Eliminating $z$ and absorbing section sizes and $T_g$ into constants $C_1,C_2>0$ and a phase $\phi_0$ gives **the leading period–parameter relation**

$$
\boxed{\mu=C_1e^{\lambda_-T}\cos(\omega T+\phi_0)
-C_2e^{-\lambda_+T}+o(e^{\lambda_-T}+e^{-\lambda_+T}).}
$$

For the idealized leading map with a constant global travel time, the displayed two terms follow exactly; for the original flow, local and global approximation errors qualify their accuracy.

If $\delta>1$, the oscillatory term is $o(z)$ and $f_S'(z)\to0$. In a sufficiently small interval the map is a contraction. For $\mu<0$ there is a unique small attracting [fixed point](../../../../../../fixed-point.md) $z=-\mu+O(|\mu|^\delta)$; it is an attracting [periodic orbit](../../../../../../periodic-orbit.md) also in the transverse direction of the full return. For $\mu\geq0$, $f_S(z)-z=-\mu-z+O(z^\delta)<0$ for sufficiently small positive $z$, so no periodic return orbit can remain wholly in this neighborhood. As $\mu\uparrow0$ from below, the attracting cycle becomes the homoclinic connection and

$$
\boxed{\mu\sim-C_2e^{-\lambda_+T},\qquad
T=\lambda_+^{-1}\log(C_2/|\mu|)+o(1).}
$$

Contraction also excludes higher-period cycles wholly inside that small return neighborhood. This does not exclude remote [periodic orbits](../../../../../../periodic-orbit.md) elsewhere in the vector field.

If $1/2<\delta<1$, the oscillatory term dominates $z$. At $\mu=0$ the fixed-point equation is

$$
\cos\theta(z)=A^{-1}z^{1-\delta}\longrightarrow0.
$$

There are infinitely many positive solutions approaching zero, with phases approaching successive zeros of cosine. Their leading ratio is $z_{j+1}/z_j\to e^{-\pi/\Omega}$, so their periods satisfy $T_{j+1}-T_j\to\pi/\omega$. At these roots the sine tends to $\pm1$, and the fixed-point multiplier has magnitude asymptotic to $A\Omega z^{\delta-1}\to\infty$. Thus these are longitudinally unstable cycles, with the thin transverse direction contracting: **infinitely many saddle [periodic orbits](../../../../../../periodic-orbit.md) accumulate on the homoclinic connection**. Expanding oscillatory lobes produce interval-covering walks and horseshoe dynamics in suitable iterates; this is the positive-saddle-value case of the [Shilnikov bifurcation](../../../../../../shilnikov-bifurcation.md).

Away from the connection, the one-passage branches wiggle in the period–parameter plane. To leading order,

$$
\boxed{\mu\sim C_1e^{\lambda_-T}\cos(\omega T+\phi_0),\qquad
|\mu|\lesssim C_1e^{\lambda_-T}.}
$$

There is no single monotone logarithmic law: the phase matters, and the exponentially smaller $-C_2e^{-\lambda_+T}$ term matters near cosine zeros. Folds occur when $f_S'(z)=1$, asymptotically at $\tan\theta=\delta/\Omega$. Their parameter values alternate in sign and accumulate geometrically toward zero. On a fixed-point branch, stability is $|f_S'(z)|<1$; small stable windows occur near stationary points of the oscillatory map. Crossing $f_S'=-1$ gives [period-doubling bifurcations](../../../../../../period-doubling-bifurcation.md), while $f_S'=1$ gives [saddle-node bifurcations of periodic orbits](../../../../../../saddle-node-bifurcation-of-periodic-orbits.md). Subsequent doublings and chaotic invariant sets can occur; neither all [periodic orbits](../../../../../../periodic-orbit.md) being stable nor a particular universal sequence for every coefficient choice is implied.

For completeness, an $m$-cycle of the return map, corresponding to a [periodic orbit](../../../../../../periodic-orbit.md) with $m$ global excursions, obeys

$$
\mu=Az_j^\delta\cos\theta(z_j)-z_{j+1}\quad(j=1,\ldots,m),\qquad z_{m+1}=z_1,
$$

and its total period is

$$
\boxed{T=mT_g+\lambda_+^{-1}\sum_{j=1}^m\log(z_0/z_j)+o(1).}
$$

Its longitudinal multiplier is $\prod_j f_S'(z_j)$. This is the relevant period relation for multipassage cycles; substituting their total $T$ into the one-passage cosine law would generally be incorrect.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
