<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Delay-compensated geometry.** Choose an east-west baseline vector $\mathbf b=b\hat{\mathbf x}$ and let the upward unit vector be $\hat{\mathbf z}$. A ray direction at zenith angle $\beta$ in their plane has $\mathbf s(\beta)=(\sin\beta,0,\cos\beta)$. Its signed geometric path difference is $\mathbf b\cdot\mathbf s=b\sin\beta$. Removing the phase-centre delay $b\sin\theta/c$ leaves the residual path

$$
\delta\ell=b[\sin(\theta+\alpha)-\sin\theta]
\simeq b\alpha\cos\theta.
$$

With the receiver ordering chosen to give positive phase for this path, a complex correlator measures

$$
\boxed{V(\alpha)\propto e^{ik\delta\ell}
\simeq\exp(ikb\alpha\cos\theta).}
$$

The reverse ordering complex-conjugates the expression without changing its information. A single real multiplier supplies its cosine component; the stated exponential represents an in-phase/quadrature correlator. Equal cable lengths to the central correlator remove a fixed instrumental difference but do not remove the changing [geometric delay](../../../../geometric-delay.md). Pointing the [antennas](../../../../antenna-radio.md) and electronically compensating the path are separate operations.

<a id="2/image-original-east-west-interferometer-geometry-and-normalized-visibility-of-a-centred-one-dimensional-uniform-source"></a>
![](../../../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1-interferometer-geometry.png)

**[Figure 2](#2/image-original-east-west-interferometer-geometry-and-normalized-visibility-of-a-centred-one-dimensional-uniform-source). Original east-west interferometer geometry and normalized visibility of a centred one-dimensional uniform source**.

**Resolved uniform source.** Contributions from mutually incoherent sky elements add as brightness-weighted [complex visibilities](../../../../complex-visibility.md). Put $I(\alpha)=I_0$ over $-\Delta\alpha/2<\alpha<\Delta\alpha/2$ and zero elsewhere, and define $q=kb\cos\theta$. Integrating gives

$$
V=I_0\int_{-\Delta\alpha/2}^{\Delta\alpha/2}e^{iq\alpha}d\alpha
=I_0\Delta\alpha\,\frac{\sin(q\Delta\alpha/2)}{q\Delta\alpha/2}.
$$

Therefore

$$
\boxed{\frac{V(b)}{V(0)}=\operatorname{sinc}\left(\frac{kb\Delta\alpha\cos\theta}{2}\right),
\qquad\operatorname{sinc}x=\frac{\sin x}{x}.}
$$

The zero-argument value is defined by continuity as one. Normalization by $V(0)=I_0\Delta\alpha$ isolates the visibility shape from total [flux](../../../../flux.md). The first null occurs when the source spans one fringe period, $\Delta\alpha=\lambda/(|b\cos\theta|)$. A negative real visibility beyond a null is a phase reversal, not negative [surface brightness](../../../../surface-brightness.md).

**Path-compensation precision.** A finite observing band sets a coherence envelope. For a rectangular band of width $\Delta\nu$, an uncorrected residual delay $\delta\tau=\delta\ell/c$ multiplies the correlation by

$$
e^{2\pi i\nu_0\delta\tau}\operatorname{sinc}(\pi\Delta\nu\delta\tau).
$$

Coarse delay steps must leave $\Delta\nu|\delta\tau|\ll1$ if decorrelation is to be small. Thus a coarse path-step scale must be well below the [coherence length](../../../../optical-coherence-length.md) $c/\Delta\nu$, with the precise bound determined by the tolerated amplitude loss and maximum quantization residual. A digital fine-delay or phase-rotation system can separately correct the central-frequency phase.

If there is no such carrier-phase correction, the steps must also be a small fraction of $\lambda$ to avoid large untracked phase jumps or time-averaging loss. For a step $d_\ell$ rounded to the nearest setting, $|\delta\ell|\le d_\ell/2$ and the maximum carrier-phase error is $\pi d_\ell/\lambda$. **[Bandwidth](../../../../bandwidth-signal-processing.md) controls coarse group-delay decorrelation; [wavelength](../../../../wavelength.md) controls the precision of untracked carrier phase.** No numerical delay step can be inferred from the central [frequency](../../../../frequency.md) alone without a [bandwidth](../../../../bandwidth-signal-processing.md), loss tolerance and compensation architecture. Earth rotation additionally sets how rapidly the delay setting must be updated.

**Largest sampled angular scale.** For a near-zenith view take the shortest projected baseline as $b_{\min}\simeq0.5\ {\rm m}$. At $\nu=30\ {\rm GHz}$, $\lambda=c/\nu=9.9931\times10^{-3}\ {\rm m}$. The inverse shortest [spatial frequency](../../../../spatial-frequency.md) gives

$$
\boxed{\Theta_{\max}\sim\frac{\lambda}{b_{\min}}
=0.0199862\ {\rm rad}=68.7\ {\rm arcmin}\approx1.15\text{ degrees}.}
$$

This is an order-of-magnitude largest fringe scale. A convention defining maximum recoverable source size as $0.6\lambda/b_{\min}$ would instead give about $41$ arcminutes; source profile, weighting and projected baseline coverage determine the operational value. The [antenna](../../../../antenna-radio.md) diameter and [primary beam](../../../../primary-beam.md) can further restrict the usable field but were explicitly neglected in the source's initial idealization. Ten [antennas](../../../../antenna-radio.md) supply $10\times9/2=45$ pairwise baselines; their number improves sampling and sensitivity, not the inverse-shortest-baseline scale by a factor of ten. The longest baseline is not supplied, so the finest synthesized resolution is not numerically fixed.

**A suitable observing programme.** A compact centimetre-wave array is well suited to [CMB](../../../../cosmic-microwave-background-split.md) temperature anisotropy on degree to sub-degree scales sampled by its baselines, and, with sufficiently long baselines and suitable foreground control, thermal Sunyaev-Zeldovich structure in [galaxy clusters](../../../../galaxy-cluster.md). At $30\ {\rm GHz}$ the thermal Sunyaev-Zeldovich signal is a decrement relative to the [CMB](../../../../cosmic-microwave-background-split.md). The compact baselines retain sensitivity to extended brightness features; the [spatial frequencies](../../../../spatial-frequency.md) measured by each baseline have a direct statistical interpretation in [CMB](../../../../cosmic-microwave-background-split.md) analysis.

Compared with lower radio [frequencies](../../../../frequency.md), synchrotron foregrounds are generally reduced, while thermal dust rises toward higher [frequencies](../../../../frequency.md); observing near this centimetre-wave atmospheric window is therefore useful, although foregrounds are not absent. Correlation and phase switching reject mean uncorrelated receiver offsets and some instrumental drifts. Receiver [thermal noise](../../../../thermal-noise.md) still contributes [variance](../../../../variance-split.md), and atmosphere, ground pickup or cross-talk can be correlated and require control. Additional long baselines can identify compact radio-source contaminants for subtraction, but the question does not specify enough array geometry to guarantee that capability. There is no zero baseline in ordinary pairwise cross-correlation, so the array does not directly measure the sky monopole or arbitrary larger-scale smooth emission.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
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
