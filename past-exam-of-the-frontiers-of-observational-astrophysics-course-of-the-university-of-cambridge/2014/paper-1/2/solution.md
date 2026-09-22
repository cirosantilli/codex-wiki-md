<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The observed population is the parent population filtered by an [astronomical selection function](../../../../astronomical-selection-function.md) and measurement errors. [Malmquist bias](../../../../malmquist-bias.md) arises because a [flux-limited galaxy selection](../../../../flux-limited-galaxy-selection.md) admits luminous objects from larger volumes: in Euclidean space $d_{\max}\propto L^{1/2}$ and $V_{\max}\propto L^{3/2}$. Thus observed [luminosity](../../../../luminosity.md) counts are weighted by $V_{\max}$. Even a nominal [standard candle](../../../../standard-candle.md) with intrinsic scatter is preferentially observed on its bright side near the limit; ignoring this can underestimate distances. A volume-limited sample or a justified $1/V_{\max}$ weighting helps, subject to completeness, geometry and evolution assumptions. Separately, [Eddington bias](../../../../eddington-bias.md) occurs when noise scatters a steeply rising population across a detection threshold: more faint objects enter than bright objects leave.

[Lutz-Kelker bias](../../../../lutz-kelker-bias.md) concerns noisy [stellar parallaxes](../../../../stellar-parallax.md) and population/selection weighting. Locally uniform spatial [density](../../../../density.md) gives $p(r)\propto r^2$ and, by changing variables, $p(\varpi)\propto\varpi^{-4}$ over the model's valid finite range. More distant [stars](../../../../star.md) are available to scatter into a parallax-limited sample than nearby [stars](../../../../star.md) to scatter out. Inverting an uncertain parallax also introduces a distinct nonlinear-estimation problem. **There is no universal magnitude correction for every [star](../../../../star.md)**: spatial [density](../../../../density.md), [luminosity](../../../../luminosity.md), [extinction](../../../../extinction.md) and how the sample was selected all matter. The classical treatment motivates this issue; it should not replace an explicit generative model.[PASP 85, 573–578; classical uniform-density calibration model](../../../../on-the-use-of-trigonometric-parallaxes-for-the-calibration-of-luminosity-systems-theory-by-t-e-lutz-and-d-h-kelker.md)

[Bayes' theorem](../../../../bayes-theorem.md) combines the measurement [likelihood function](../../../../likelihood-function.md) with a justified [prior distribution](../../../../prior-probability.md). For example, with a [Gaussian](../../../../normal-distribution.md) parallax error and consistent distance/parallax units,

$$
p(r\mid\widehat\varpi)\propto
\exp\!\left[-\frac{(\widehat\varpi-1/r)^2}{2\sigma_\varpi^2}\right]p(r),\qquad r>0.
$$

A [proper distance prior for parallax inference](../../../../proper-distance-prior-for-parallax-inference.md) might have $p(r)\propto r^2e^{-r/L}$ with a justified scale $L$; extending $r^2$ to infinity gives an improper [posterior](../../../../bayesian-posterior.md) here. Negative measured parallaxes remain valid noisy data. For [selection conditioning in Bayesian inference](../../../../selection-conditioning-in-bayesian-inference.md), distinguish individual inference from population inference: if selection is determined entirely by the exact data already conditioned on, it adds no further information about that individual's parameters. For population parameters $\Lambda$, the selected-data [likelihood](../../../../likelihood-function.md) must instead include the detection normalization $\alpha(\Lambda)=\int S(d)p(d\mid\Lambda)\,dd$. Applying a cut twice is also an error.

Selection can depend on [surface brightness](../../../../surface-brightness.md), [angular resolution](../../../../angular-resolution.md), dust, sky coverage, colour and observing cadence as well as total flux. Crowding and unresolved binaries bias distance calibrators. Transit surveys favour large [planets](../../../../planet.md) and short periods, with an additional geometric transit probability approximately $R_\star/a$ for small [planets](../../../../planet.md) on circular orbits; injection/recovery tests quantify the remaining [transit survey completeness](../../../../transit-survey-completeness.md). Cluster catalogues select noisy mass proxies from a steep abundance distribution. Planck's 2013 SZ catalogue explicitly characterized detection completeness and reliability rather than identifying every detection with an unbiased mass census.[abstract and selection-function/completeness analysis, 2013 preprint](../../../../planck-2013-results-xxix-planck-catalogue-of-sunyaev-zeldovich-sources-by-planck-collaboration.md) Calibrators, artificial-source tests and a forward model of detection, measurement and follow-up are the practical checks on any correction.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
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
