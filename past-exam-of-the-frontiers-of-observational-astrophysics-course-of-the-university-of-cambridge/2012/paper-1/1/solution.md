<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The geometric path difference for a direction at zenith angle $\theta+\alpha$ is $b\sin(\theta+\alpha)$. Equal cable lengths leave that difference unchanged; the inserted electronic delay cancels $b\sin\theta$ for the tracking center. The residual delay is therefore

$$
\tau=\frac bc[\sin(\theta+\alpha)-\sin\theta]\simeq\frac{b\alpha\cos\theta}{c}.
$$

The [complex visibility](../../../../complex-visibility.md) of the unresolved source has phase $2\pi\nu\tau$, giving $\exp(ikb\alpha\cos\theta)$ in the chosen baseline ordering. Reversing the signal order complex-conjugates it without changing the measured visibility magnitude. Tracking the [antennas](../../../../antenna-radio.md) geometrically does not itself provide this [fringe stopping](../../../../fringe-stopping.md).

<a id="1/image-tracking-delay-in-a-two-antenna-interferometer"></a>
![](../../../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2012/paper-1-interferometer-delay.png)

**[Figure 1](#1/image-tracking-delay-in-a-two-antenna-interferometer). Tracking delay in a two-antenna interferometer**. Original functional schematic. The nearer antenna receives the tracked wave earlier and its electronic delay compensates that geometric lead. Angles are exaggerated and cable paths are schematic.

For a top-hat band centered at $\nu_0$, let $f=\nu-\nu_0$. Averaging the residual fringe gives

$$
\frac1{\Delta\nu}\int_{-\Delta\nu/2}^{\Delta\nu/2}e^{2\pi i(\nu_0+f)\tau}\,df
=e^{2\pi i\nu_0\tau}\operatorname{sinc}(\pi\Delta\nu\tau),
\qquad\operatorname{sinc}x=\frac{\sin x}{x}.
$$

After removing the central fringe phase, its envelope is exactly

$$
\boxed{\operatorname{sinc}\left(\frac{\pi\Delta\nu b\alpha\cos\theta}{c}\right).}
$$

The full complex average retains the displayed central-frequency phase; the bare sinc in the question is the phase-referenced envelope or an average written in frequency-offset coordinates. This [bandwidth decorrelation of a point source](../../../../bandwidth-decorrelation-of-a-point-source.md) is cancellation between different frequency-dependent phases, not absorption of source radiation.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../split.md)
5. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
