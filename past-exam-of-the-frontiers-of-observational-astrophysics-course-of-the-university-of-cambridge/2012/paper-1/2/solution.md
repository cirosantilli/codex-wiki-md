<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An observed catalogue is the result of a population, an instrument and a selection rule. Its [astronomical selection function](../../../../astronomical-selection-function.md) can depend on [flux](../../../../flux.md), color, size, [surface brightness](../../../../surface-brightness.md), sky location, cadence and follow-up success. The relevant cut is often on noisy measured quantities. A model that selects on noiseless true [flux](../../../../flux.md) instead can predict a different sample even when it uses the same nominal threshold.

[Malmquist bias](../../../../malmquist-bias.md) occurs because brighter members of a population are visible through a larger [volume](../../../../volume.md) in a flux-limited survey. For a uniform Euclidean population, $r_{\max}\propto\sqrt L$ and $V_{\max}\propto L^{3/2}$. The selected [luminosity](../../../../luminosity.md) distribution is therefore weighted toward large $L$. For an intrinsic [Gaussian](../../../../normal-distribution.md) absolute-magnitude distribution with [mean](../../../../expected-value-split.md) $M_0$ and [variance](../../../../variance-split.md) $\sigma_M^2$, multiplying by $10^{-0.6M}$ and completing the square gives the [Gaussian absolute-magnitude Malmquist shift](../../../../gaussian-absolute-magnitude-malmquist-shift.md)

$$
\boxed{\langle M\rangle_{\rm selected}=M_0-0.6\ln(10)\,\sigma_M^2
\simeq M_0-1.382\sigma_M^2.}
$$

This assumes the stated simple population, a complete [flux](../../../../flux.md) cut and no additional boundaries. Exactly identical noiseless [standard candles](../../../../standard-candle.md) have a distance truncation, not a [luminosity](../../../../luminosity.md) spread to reweight. Scatter, [extinction](../../../../extinction.md), cosmological [volume](../../../../volume.md) and source evolution need their own model.

[Lutz-Kelker bias](../../../../lutz-kelker-bias.md) concerns parallax errors, spatial population weighting and selected [calibration](../../../../calibration-differential-geometry.md) samples. Uniform spatial [density](../../../../density.md) gives $p(r)\propto r^2$ locally, hence $p(\varpi)\propto\varpi^{-4}$ on the physically valid range. More distant objects can scatter into a measured-parallax cut. In addition, inversion $r=1/\widehat\varpi$ is nonlinear and gives misleading estimates at low signal-to-noise; a negative measured parallax is possible even for a positive true distance. A [posterior](../../../../bayesian-posterior.md) instead combines the parallax [likelihood](../../../../likelihood-function.md) with a justified population [prior](../../../../prior-probability.md). An unbounded uniform-volume [prior](../../../../prior-probability.md) is improper here; a finite population model or a [proper distance prior for parallax inference](../../../../proper-distance-prior-for-parallax-inference.md) is necessary.[classical selected-sample parallax-calibration model](../../../../on-the-use-of-trigonometric-parallaxes-for-the-calibration-of-luminosity-systems-theory-by-t-e-lutz-and-d-h-kelker.md)

[Bayes' theorem](../../../../bayes-theorem.md) makes the assumptions explicit. If $\eta$ denotes population parameters, $x$ latent properties and $S$ the catalogue inclusion event, a selected-sample [likelihood](../../../../likelihood-function.md) has the form

$$
p(d\mid\eta,S)=\frac{\mathbf1_S(d)\int p(d\mid x)p(x\mid\eta)\,dx}
{\int_{d'\in S}\!dd'\int p(d'\mid x)p(x\mid\eta)\,dx}.
$$

This [selection-normalized astronomical likelihood](../../../../selection-normalized-astronomical-likelihood.md) accounts for the model-dependent [probability](../../../../probability.md) of entering the catalogue. For individual inference, selection information already determined by the fully conditioned measured data must not be multiplied in a second time. The sampling design, inferential target and actual conditioned information determine the appropriate expression.

Other effects include [Eddington bias](../../../../eddington-bias.md), where steep number counts and measurement scatter move more faint objects upward than bright objects downward, and surface-brightness selection that misses diffuse galaxies despite substantial total [flux](../../../../flux.md). Dust [extinction](../../../../extinction.md) affects both detectability and inferred [luminosity](../../../../luminosity.md). Variable-source detection depends on cadence and duration; spectroscopic follow-up can favor easy-to-measure redshifts or particular colors. Blends, [calibration](../../../../calibration-differential-geometry.md) drift and redshift errors can mimic population changes.

Examples include magnitude-limited supernova samples used in distance-redshift fits, where [luminosity](../../../../luminosity.md) scatter and follow-up must be modeled, and radial-velocity planet surveys, which favor large-amplitude, short-period systems and leave inclination degeneracies. Forward modeling through the survey pipeline, injection-and-recovery estimates of completeness, calibrated [noise](../../../../noise-signal-processing.md) and properly modeled censored or nondetected observations address these effects. A universal correction or an unexamined inverse-volume weight does not replace an explicit generative and selection model.

## ↑ Ancestors (13)

1. [2](../2.md)
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
