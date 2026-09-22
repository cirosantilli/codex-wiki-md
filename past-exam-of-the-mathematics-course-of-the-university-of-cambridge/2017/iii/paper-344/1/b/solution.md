<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $\Gamma>0$ is a [kinetic coefficient](../../../../../../kinetic-coefficient.md), and the additive [Gaussian white noise](../../../../../../gaussian-white-noise.md) must be centered. A rigorous starting point is a finite spatial discretization or finite set of modes of the coarse-grained field. For each field coordinate, the [Fokker-Planck probability current](../../../../../../fokker-planck-probability-current.md) has the continuum notation

$$
\mathcal J(\mathbf r;[\phi])=-\Gamma\frac{\delta F}{\delta\phi(\mathbf r)}\mathcal P[\phi]-\frac{\sigma^2}{2}\frac{\delta\mathcal P}{\delta\phi(\mathbf r)}.
$$

The equilibrium [Boltzmann distribution](../../../../../../boltzmann-distribution.md) $\mathcal P_{\rm eq}\propto e^{-\beta F}$ has $\delta\mathcal P_{\rm eq}/\delta\phi=-\beta(\delta F/\delta\phi)\mathcal P_{\rm eq}$. [Detailed balance](../../../../../../detailed-balance.md) for this time-even field requires zero configuration-space current. Therefore

$$
\mathcal J_{\rm eq}=\left(-\Gamma+\frac{\beta\sigma^2}{2}\right)\frac{\delta F}{\delta\phi}\mathcal P_{\rm eq}=0,\qquad \boxed{\sigma^2=2\Gamma k_BT.}
$$

This is the [Model A fluctuation-dissipation relation](../../../../../../model-a-fluctuation-dissipation-relation.md). Conversely, that noise strength makes the equilibrium current vanish and gives reversible relaxational dynamics when the equilibrium measure is normalizable.

Alternatively, the [Onsager--Machlup path probability for Model A dynamics](../../../../../../onsager-machlup-path-probability-for-model-a-dynamics.md) compares the squared required noise histories $\dot\phi+\Gamma\delta F/\delta\phi$ and $-\dot\phi+\Gamma\delta F/\delta\phi$. Their difference gives $\log(\mathbb P_F/\mathbb P_B)=-2\Gamma\Delta F/\sigma^2$, using the [functional chain rule](../../../../../../functional-chain-rule.md). The midpoint convention and [time-reversal invariance of a path Jacobian](../../../../../../time-reversal-invariance-of-a-path-jacobian.md) justify cancellation of the common Jacobian. Comparing with the conditional path ratio gives the same result. The spatial white-noise continuum is a coarse-grained idealization: retain a microscopic cutoff when pointwise fluctuations or ultraviolet divergences matter.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
