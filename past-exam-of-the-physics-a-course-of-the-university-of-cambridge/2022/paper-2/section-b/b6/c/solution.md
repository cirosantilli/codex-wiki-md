<h1 id="section-b/b6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The natural interpretation is the fundamental transverse [normal mode](../../../../../../normal-mode.md), $n=1$. Indeed

$$
\omega_{c,1}=\frac{\pi v}{b}=62.832\,\mathrm{rad\,s^{-1}},\qquad
\omega_{c,2}=125.66\,\mathrm{rad\,s^{-1}},
$$

so only $n=1$ propagates over the main part of the given [Gaussian distribution](../../../../../../normal-distribution.md) of [angular frequencies](../../../../../../angular-frequency.md). Its centre travels at

$$
v_{g,0}=2\sqrt{1-(62.832/100)^2}=1.5559\,\mathrm{m\,s^{-1}},\qquad
t_0=\frac{10\,\mathrm m}{v_{g,0}}=6.4271\,\mathrm s.
$$

Differentiate the [group velocity](../../../../../../group-velocity.md) with respect to [angular frequency](../../../../../../angular-frequency.md):

$$
\frac{dv_g}{d\omega}
=\frac{v\omega_c^2}{\omega^3\sqrt{1-(\omega_c/\omega)^2}}.
$$

At the centre this is $0.010149\,\mathrm m$. The one-standard-deviation [group velocity](../../../../../../group-velocity.md) spread is consequently

$$
\sigma_v\simeq\left|\frac{dv_g}{d\omega}\right|_{\omega_0}\sigma_\omega
=0.05075\,\mathrm{m\,s^{-1}}.
$$

Over the central travel time the associated spatial shear is

$$
\boxed{\sigma_{x,\rm disp}\simeq t_0\sigma_v=0.326\,\mathrm m.}
$$

Equivalently, use representative components at $\omega_0\pm\sigma_\omega$, for which $v_g(95)=1.5001\,\mathrm{m\,s^{-1}}$ and $v_g(105)=1.6024\,\mathrm{m\,s^{-1}}$. Their separation after $t_0$ is

$$
\boxed{\Delta x_{[-\sigma,+\sigma]}\simeq[v_g(105)-v_g(95)]t_0=0.658\,\mathrm m\simeq0.65\,\mathrm m.}
$$

At a fixed detector $10\,\mathrm m$ away, the corresponding arrival-time difference is $10/v_g(95)-10/v_g(105)=0.426\,\mathrm s$.

The paper asks for an estimate of spreading, without specifying a spatial width convention or the initial spectral [phase](../../../../../../phase-waves.md). A [Gaussian distribution](../../../../../../normal-distribution.md) has no finite full range. Thus $0.326\,\mathrm m$ is a one-standard-deviation dispersive contribution, whereas about $0.65\,\mathrm m$ describes the separation of the $\pm\sigma_\omega$ representatives. Neither is automatically the increase in the packet's original width. For an initially unchirped [Gaussian wave packet](../../../../../../gaussian-wave-packet.md) in the narrow-band approximation, independent initial and dispersive contributions combine as $\sigma_{x,f}^2\simeq\sigma_{x,0}^2+\sigma_{x,\rm disp}^2$; a packet with an initial [chirp](../../../../../../chirp.md) can behave differently. The modal assumption and width convention must accompany the numerical answer.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
