<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A conceptual single-molecule measurement follows a labelled bound molecule along an independently mapped [DNA](../../../../deoxyribonucleic-acid.md) contour. Project fitted positions onto contour distance and estimate the [mean-squared displacement](../../../../mean-squared-displacement.md) at several lag times. For unbiased [one-dimensional diffusion](../../../../diffusion.md),

$$
\langle[s(t+\Delta t)-s(t)]^2\rangle=2D_1\Delta t.
$$

Independent localization errors of [variance](../../../../variance-split.md) $\sigma_{\rm loc}^2$ add an intercept $2\sigma_{\rm loc}^2$. Finite exposure adds motion blur, and [drift](../../../../drift-velocity.md), binding transitions and the finite [DNA](../../../../deoxyribonucleic-acid.md) contour must be distinguished from free [sliding](../../../../facilitated-target-search.md). A slope fit with those limitations can estimate $D_1$; simply fitting all observed [displacements](../../../../displacement.md) to a noiseless line can bias it.

**Retain the printed coefficient.** The original PDF really prints $D_1=5\times10^{10}\,\mathrm{m^2\,s^{-1}}$, not a negative exponent. In [sliding diffusivity with per-step dissociation](../../../../sliding-diffusivity-with-per-step-dissociation.md), for a basepair step $a\simeq0.34\,\mathrm{nm}$, an [unbiased nearest-neighbour walk](../../../../random-walk-split.md) has step interval $a^2/(2D_1)$. If the [dissociation](../../../../dissociation-rate-constant.md) [probability](../../../../probability.md) per step is $P$, the mean number of steps is approximately $1/P$, giving

$$
\boxed{\tau_{\rm bound}\simeq\frac{a^2}{2D_1P},\qquad
\ell_{\rm rms}\simeq\frac a{\sqrt P}.}
$$

For the printed values, $\tau_{\rm bound}\simeq1.16\times10^{-24}\,\mathrm s$ and $\ell_{\rm rms}\simeq0.34\,\mathrm{\mu m}$. The latter is a random-walk [displacement](../../../../displacement.md), not the contour distance travelled in a million steps. The step interval is about $1.16\times10^{-30}\,\mathrm s$, even shorter than the light-travel time across a basepair by many orders of magnitude. This is an unphysical extrapolation for a [protein](../../../../protein-split.md), not a meaningful experimentally measurable [diffusivity](../../../../diffusion-coefficient.md).

Consequently no [fluorescence](../../../../fluorescence-split.md) camera could temporally resolve trajectories under the stated formal values, regardless of the spatial excursion's length. An actual corrected exponent cannot be inferred uniquely from the paper. If a physically plausible $D_1$ were supplied instead, resolving [sliding](../../../../facilitated-target-search.md) would require exposures substantially shorter than $\tau_{\rm bound}$ and [diffusion](../../../../diffusion.md) [displacements](../../../../displacement.md) larger than [localization error](../../../../measurement-error.md), with enough detected [photons](../../../../photon.md). The dependence on $D_1$ is explicit above, so no guessed source correction is needed.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
