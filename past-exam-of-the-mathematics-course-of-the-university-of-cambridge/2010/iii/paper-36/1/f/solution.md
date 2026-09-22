<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Substituting the standardized deviation into the [Bayes factor](../../../../../../bayes-factor.md) approximation gives

$$
\boxed{B_{01}\approx\sqrt{\frac{20000}{\pi}}e^{-4.5}\approx0.89,\qquad B_{10}\approx1.13.}
$$

This is only a slight preference for the alternative, despite the small [p-value](../../../../../../p-value.md). The two procedures measure different things: the [p-value](../../../../../../p-value.md) sums a tail under the [null hypothesis](../../../../../../null-hypothesis.md), while the [Bayes factor](../../../../../../bayes-factor.md) compares probabilities of the observed count under both models. The uniform alternative [prior distribution](../../../../../../prior-probability.md) spreads its probability over many success probabilities that fit the observations poorly. Only a narrow range around $0.515$ has large [likelihood](../../../../../../likelihood-function.md), and integrating over the whole alternative penalizes this diffuse prediction.

The prefactor makes the distinction especially clear. At a fixed standardized deviation $z$, the [p-value](../../../../../../p-value.md) stays approximately $2\{1-\Phi(|z|)\}$, whereas $B_{01}\approx\sqrt{2n/\pi}e^{-z^2/2}$ eventually grows with $n$. A fixed diffuse alternative can consequently favour the point null even while a conventional test rejects it. This is the same prior-width mechanism illustrated by the [Jeffreys-Lindley paradox for a Gaussian point null](../../../../../../jeffreys-lindley-paradox-for-a-gaussian-point-null.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
