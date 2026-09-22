<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a full [Euclidean lattice](../../../../../../euclidean-lattice.md) $\Lambda\subseteq\mathbb R^n$, its [dual lattice](../../../../../../dual-lattice.md) is

$$
\Lambda^\vee=\{y:\langle x,y\rangle\in\mathbb Z\text{ for every }x\in\Lambda\}.
$$

For a Schwartz function, the [Poisson summation formula for a Euclidean lattice](../../../../../../poisson-summation-formula-for-a-euclidean-lattice.md) states

$$
\sum_{\lambda\in\Lambda}f(\lambda)
=m(\Lambda)^{-1}\sum_{\mu\in\Lambda^\vee}\widehat f(\mu),
\qquad
\widehat f(y)=\int_{\mathbb R^n}f(x)e^{-2\pi i\langle x,y\rangle}\,dx.
$$

To prove it, periodize $f$ over $\Lambda$. The resulting function on $\mathbb R^n/\Lambda$ has Fourier coefficient $m(\Lambda)^{-1}\widehat f(\mu)$ at $\mu\in\Lambda^\vee$. Evaluating its absolutely convergent Fourier series at zero gives the identity. The same proof applies under the usual weaker hypotheses ensuring convergence of both sides.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
