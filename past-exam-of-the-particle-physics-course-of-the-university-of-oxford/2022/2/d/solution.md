<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The long-lived, electrically neutral [kaon](../../../../kaon.md) often traverses the [particle detector](../../../../particle-detector.md) without decaying into a reconstructable charged final state. Identifying it through a hadronic interaction or missing [four-momentum](../../../../four-momentum.md) is much less efficient than reconstructing the short-lived [kaon](../../../../kaon.md) through its nearby two-[pion](../../../../pion.md) [decay vertex](../../../../decay-vertex.md). The efficiencies must be applied to the observed counts before taking their asymmetry:

$$
N_S=\frac{1107}{0.93}=1190.32,\qquad N_L=\frac{49}{0.05}=980,
\qquad \mathcal R=\frac{N_S-N_L}{N_S+N_L}=0.09691.
$$

Using the leading aligned-amplitude approximation from [c](../c.md),

$$
\boxed{\theta_C=\arctan\sqrt{\mathcal R/2}=0.21667\ \mathrm{rad}=12.41^\circ.}
$$

The exact aligned formula instead gives $12.43^\circ$, an immaterial correction here. Treating the observed counts as independent [Poisson random variables](../../../../poisson-distribution.md) and the efficiencies as known, [propagation of uncertainty](../../../../propagation-of-uncertainty.md) gives

$$
\sigma_S=\frac{\sqrt{1107}}{0.93}=35.78,\qquad \sigma_L=\frac{\sqrt{49}}{0.05}=140,
$$



$$
\sigma_{\mathcal R}^2=\left[\frac{2N_L}{(N_S+N_L)^2}\right]^2\sigma_S^2+
\left[\frac{2N_S}{(N_S+N_L)^2}\right]^2\sigma_L^2,
\qquad \boxed{\sigma_{\mathcal R}=0.0723.}
$$

The separate contributions to $\sigma_{\mathcal R}$ are $0.0149$ and $0.0708$; the small $K_L$ sample dominates. Linear [propagation of uncertainty](../../../../propagation-of-uncertainty.md) yields $\sigma(\theta_C)\simeq4.49^\circ$, although the nonlinear extraction and physical boundary make a symmetric [confidence interval](../../../../confidence-interval.md) a rough summary. Unknown efficiency uncertainties, especially that of $K_L$, would be additional systematic contributions.

The supplied [CKM matrix](../../../../cabibbo-kobayashi-maskawa-matrix.md) gives $\sin\theta_C\simeq0.224$, hence $\theta_C\simeq12.94^\circ$ and $\mathcal R\simeq2(0.224/0.975)^2=0.1056$. The asymmetry difference is only about $0.12$ statistical [standard deviations](../../../../standard-deviation.md), so the measurement is compatible. Without the phase assumption, these data measure $\tan^2\theta_C\cos\delta$ to leading order and do not uniquely measure the [Cabibbo angle](../../../../cabibbo-angle.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
