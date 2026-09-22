<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[PALM](../../../../photoactivated-localization-microscopy.md) separates emitters in time. A sparse subset of photoactivatable or photoconvertible labels is switched on so that its diffraction-broadened images can be fitted individually; repeated activation, imaging and localization builds a map from many isolated detections. The positional uncertainty can be much smaller than the [point spread function](../../../../point-spread-function-split.md) width because many [photons](../../../../photon.md) estimate one image centre: ideally $\sigma_{\rm loc}\sim s/\sqrt{N_\gamma}$ for image width $s$ and detected [photon](../../../../photon.md) number $N_\gamma$.

That is [fluorescence localization precision](../../../../fluorescence-localization-precision.md), not automatically the structural resolution of the reconstructed cell. Pixelation, background, imperfect optics, drift, label linkage, blinking and labelling density matter. Repeated localizations of one molecule cannot fill unlabelled gaps; a crowded frame with overlapping images cannot simply be treated as many isolated emitters. For a static structural map, the structure must remain sufficiently stable while the many frames are accumulated, or its time dependence must be reconstructed explicitly.

For mobility in living cells, keep activated [proteins](../../../../protein-split.md) observable for successive frames and link isolated positions into trajectories before bleaching. Repeating this for successive sparse subsets yields many trajectories without making the entire [protein](../../../../protein-split.md) population simultaneously fluorescent. This is the [sptPALM](../../../../single-particle-tracking-palm.md) strategy.[Combination of sparse photoactivation and live-cell single-particle tracking](../../../../high-density-mapping-of-single-molecule-trajectories-with-photoactivated-localization-microscopy-by-suliana-manley-and-others.md)

For free isotropic two-dimensional [diffusion](../../../../diffusion.md) with per-coordinate localization error $\sigma_{\rm loc}$ and instantaneous exposures,

$$
\boxed{\langle|\mathbf r(t+\Delta t)-\mathbf r(t)|^2\rangle
=4D\Delta t+4\sigma_{\rm loc}^2.}
$$

Fit several lags or a full trajectory [likelihood](../../../../likelihood-function.md) to infer D and its uncertainty. Finite exposure causes [motion blur](../../../../motion-blur.md); for a uniform shutter of duration $t_E\le\Delta t$, a simple correction is $4D(\Delta t-t_E/3)+4\sigma_{\rm loc}^2$. Confinement, directed motion and switching binding states change the lag dependence. Short tracks, missed detections and false linking in crowded regions can mimic apparent heterogeneity, so mobility classes require explicit measurement-error and tracking controls. A trajectory map recovers dynamics; it is not identical to a static [PALM](../../../../photoactivated-localization-microscopy.md) density map.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
