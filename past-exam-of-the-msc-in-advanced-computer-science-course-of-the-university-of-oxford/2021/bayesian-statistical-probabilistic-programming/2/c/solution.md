<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The discrete base factors in the displayed construction inherit their variational parameters. Accordingly write **$s_\lambda(\varepsilon)$**, not a parameter-independent $s(\varepsilon)$, for the joint base [probability mass function](../../../../../probability-mass-function.md) or [probability density function](../../../../../probability-density-function.md). The continuous noise factors can be parameter independent while the discrete factors are $\lambda$ dependent. Calling the entire base law parameterless while retaining its nonzero [score function](../../../../../informant-function.md) would be inconsistent.

Let $t_\lambda$ push the base law forward to $q_\lambda$, and define

$$
W_\lambda(\varepsilon,x)=\log p(t_\lambda(\varepsilon),x)-\log q_\lambda(t_\lambda(\varepsilon)).
$$

Use a fixed base [measure](../../../../../measure-split.md) $\nu$, with [counting measure](../../../../../counting-measure.md) for discrete coordinates and [Lebesgue measure](../../../../../lebesgue-measure.md) for continuous coordinates. Assume locally parameter-independent support, differentiability and an integrable domination permitting [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md). A valid [reparameterization gradient](../../../../../reparameterization-gradient.md) gives

$$
\mathcal L(\lambda)=\int s_\lambda(\varepsilon)W_\lambda(\varepsilon,x)\,d\nu(\varepsilon).
$$

Apply the [product rule](../../../../../product-rule.md) before simplifying:

$$
\begin{aligned}
\nabla_\lambda\mathcal L
&=\int\left[(\nabla_\lambda s_\lambda)W_\lambda+s_\lambda\nabla_\lambda W_\lambda\right]d\nu\\
&=\mathbb E_{s_\lambda}\left[(\nabla_\lambda\log s_\lambda(\varepsilon))W_\lambda(\varepsilon,x)+\nabla_\lambda W_\lambda(\varepsilon,x)\right]\\
&=\mathbb E_{s_\lambda}\left[(\nabla_\lambda\log s_\lambda(\varepsilon))W_\lambda(\varepsilon,x)+\nabla_\lambda\log p(t_\lambda(\varepsilon),x)-\nabla_\lambda\log q_\lambda(t_\lambda(\varepsilon))\right].
\end{aligned}
$$

This is the required [combined score and pathwise gradient estimator](../../../../../combined-score-and-pathwise-gradient-estimator.md). A sample from $s_\lambda$ and the integrand on the last line give an [unbiased stochastic gradient](../../../../../unbiased-stochastic-gradient.md) under the stated regularity conditions. Its first term is a [score-function gradient estimator](../../../../../score-function-gradient-estimator.md) contribution; the remaining terms differentiate the sampled objective along the continuous transformation. The same separation appears in the general [stochastic computation graph](../../../../../stochastic-computation-graph.md) construction.[Section 3.1, Theorem 1, equations (5)–(6); Appendix A](../../../../../gradient-estimation-using-stochastic-computation-graphs-by-john-schulman-and-others.md)

All derivatives inside the [expectation](../../../../../expected-value-split.md) hold $\varepsilon$ fixed. They still include both explicit parameter dependence and dependence through $t_\lambda$. For a continuous coordinate $z=t_\lambda(\varepsilon)$,

$$
\nabla_\lambda\log q_\lambda(t_\lambda(\varepsilon))=(\partial_\lambda\log q_\lambda)(z)+(D_\lambda t_\lambda)^T\nabla_z\log q_\lambda(z).
$$

The model joint density $p(z,x)$ is fixed as $\lambda$ changes, but its composition with $t_\lambda$ need not be constant. Discrete coordinates are not differentiated as real-valued paths; their changing [probabilities](../../../../../probability.md) enter through the [score function](../../../../../informant-function.md). Moving supports or parameter-dependent branch boundaries require additional care and are not justified merely by formally interchanging a derivative and an integral.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
