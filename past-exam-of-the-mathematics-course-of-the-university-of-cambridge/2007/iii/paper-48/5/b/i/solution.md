<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $S_m=\sum_{i=1}^m x_i$ and $S=S_N$. Use shape-rate notation for the [Gamma distribution](../../../../../../../gamma-distribution.md), as in the authoritative PDF: shape $a$ and rate $b$ give a density proportional to $z^{a-1}e^{-bz}$. Conditional independence of the [Poisson distributions](../../../../../../../poisson-distribution.md) gives a [likelihood function](../../../../../../../likelihood-function.md) proportional to

$$
\lambda^{S_m}e^{-m\lambda}\phi^{S-S_m}e^{-(N-m)\phi}.
$$

The product of factorial terms depends only on the data and can be absorbed into the normalizing constant. Multiplying by the two independent [Gamma distribution](../../../../../../../gamma-distribution.md) prior kernels and the uniform prior on the possible indices gives the [Poisson count change-point model with gamma priors](../../../../../../../poisson-count-change-point-model-with-gamma-priors.md):

$$
\boxed{\pi(\lambda,\phi,m\mid x)\propto\lambda^{\alpha+S_m-1}e^{-(\beta+m)\lambda}\phi^{\gamma+S-S_m-1}e^{-(\delta+N-m)\phi}\,\mathbf1_{\{\lambda>0,\phi>0,\ m\in\{1,\ldots,N\}\}}.}
$$

Because the hyperparameters are positive, each possible index gives finite positive gamma integrals, and summing over the finitely many indices yields a proper [posterior distribution](../../../../../../../bayesian-posterior.md). At $m=N$ the second likelihood factor is one, so the posterior law of its unused rate $\phi$ remains its prior $\operatorname{Gamma}(\gamma,\delta)$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 48](../../../../paper-48-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
