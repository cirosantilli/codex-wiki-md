<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Condition on the observed value $X=x$. If a classifier reports class zero, its conditional probability of error is $\mathbb P(Y=1\mid X=x)$; if it reports class one, the conditional error is $\mathbb P(Y=0\mid X=x)$. Therefore the smaller conditional error is attained by class one exactly when

$$
\pi_1f_1(x)>\pi_0f_0(x),
$$

and by class zero exactly when the reverse strict inequality holds. Integrating these pointwise conditional errors proves that $\delta_{\pi_0}$ is a [Bayes classifier](../../../../../../bayes-classifier.md).

The only possible nonuniqueness lies on the tie set

$$
B=\{x:\pi_1f_1(x)=\pi_0f_0(x)\}
=\{x:D_{\pi_0}(x)=0\}.
$$

Because the two Gaussian class distributions are distinct, $D_{\pi_0}$ is not identically zero. It is a nonzero polynomial of degree at most two, so its zero set has [Lebesgue measure](../../../../../../lebesgue-measure.md) zero. Both Gaussian laws have densities with respect to Lebesgue measure, hence assign probability zero to $B$. Every Bayes rule must therefore agree with $\delta_{\pi_0}$ almost surely. This proves the [uniqueness of a Bayes classifier](../../../../../../uniqueness-of-a-bayes-classifier.md) up to the standard null-set equivalence of decision rules.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
