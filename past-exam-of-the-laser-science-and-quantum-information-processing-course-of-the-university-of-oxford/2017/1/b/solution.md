<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $v_g\simeq c/n_r$ be the light's [group velocity](../../../../group-velocity.md) in the fibre, with unit mode overlap and a uniform transverse mode area. The [fibre-laser gain-volume rate equations](../../../../fibre-laser-gain-volume-rate-equations.md) follow because the upper-level [density](../../../../density.md) is defined per doped volume, whereas the [photon](../../../../photon.md) [density](../../../../density.md) is defined per full cavity volume. [Stimulated emission](../../../../stimulated-emission.md) therefore removes upper-level ions at rate $v_g\sigma_{21}N_2n$ per doped volume, but supplies cavity [photons](../../../../photon.md) at the volume-averaged rate $fv_g\sigma_{21}N_2n$. Thus

$$
\dot N_2=S-v_g\sigma_{21}N_2n-\frac{N_2}{\tau_2},\qquad
\dot n=\left(fv_g\sigma_{21}N_2-\frac1{\tau_c}\right)n.
$$

At threshold the stimulated [photon](../../../../photon.md) growth rate balances the [photon](../../../../photon.md) loss rate, giving

$$
\boxed{N_{\mathrm{th}}=\frac1{fv_g\sigma_{21}\tau_c}\simeq\frac{n_r}{fc\sigma_{21}\tau_c}.}
$$

Using this relation yields the stated equations, including the essential $1/f$ in the ion-depletion term:

$$
\dot N_2=S-\frac1f\frac{N_2}{N_{\mathrm{th}}}\frac n{\tau_c}-\frac{N_2}{\tau_2},\qquad
\dot n=\left(\frac{N_2}{N_{\mathrm{th}}}-1\right)\frac n{\tau_c}.
$$

Above threshold, the nonzero stationary [photon](../../../../photon.md) [density](../../../../density.md) requires $N_{2,\mathrm{ss}}=N_{\mathrm{th}}$. The remaining stationary equation then gives

$$
\boxed{r=\frac{S\tau_2}{N_{\mathrm{th}}}=\frac S{S_{\mathrm{th}}},\qquad
n_{\mathrm{ss}}=(r-1)f\frac{\tau_c}{\tau_2}N_{\mathrm{th}},\qquad S_{\mathrm{th}}=\frac{N_{\mathrm{th}}}{\tau_2}.}
$$

The parameter $r$ is the pump rate in units of its lasing-threshold value. The above-threshold branch requires $r>1$; below threshold the ideal stationary solution is $n=0$, $N_2=S\tau_2$. [Spontaneous emission](../../../../spontaneous-emission.md) into the lasing mode has been omitted in this deterministic model, so an exactly zero initial field would need a seed or noise to start, even when the zero-field branch is unstable.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
