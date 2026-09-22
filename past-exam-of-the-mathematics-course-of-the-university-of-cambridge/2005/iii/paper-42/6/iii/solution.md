<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $I_n=\int_{\mathbb R^p}e^{nh(\theta)}a(\theta)d\theta$, suppose $h$ has a unique interior maximum $\widehat\theta$, $H=-h''(\widehat\theta)$ is positive definite, the amplitude is smooth there, and contributions away from that maximum are negligible. Set $z=\sqrt n(\theta-\widehat\theta)$. The quadratic expansion $nh(\theta)=nh(\widehat\theta)-z^THz/2+o(1)$ yields the [Laplace approximation](../../../../../../laplace-approximation.md)

$$
\boxed{I_n\sim e^{nh(\widehat\theta)}a(\widehat\theta)(2\pi/n)^{p/2}|H|^{-1/2}.}
$$

The determinant comes from diagonalizing the [Gaussian integral](../../../../../../gaussian-integral.md); it is an inverse square root, not an inverse determinant. Under standard higher smoothness and domination, the relative error is $O(n^{-1})$.

For a regular model and a fixed smooth positive proper prior $\pi$, apply this to the [marginal likelihood](../../../../../../bayesian-model-evidence.md) $m(y)=\int e^{\ell(\theta;y)}\pi(\theta)d\theta$. With $j(\widehat\theta)=-\ell''(\widehat\theta)$,

$$
m(y)\approx e^{\ell(\widehat\theta)}\pi(\widehat\theta)(2\pi)^{p/2}|j(\widehat\theta)|^{-1/2}.
$$

As $j$ is of order $n$, this produces the $p\log n$ complexity term in the [Bayesian information criterion](../../../../../../bayesian-information-criterion.md) after multiplying log [marginal likelihood](../../../../../../bayesian-model-evidence.md) by $-2$. A posterior mode can also be used with the corresponding combined log-density curvature. Boundary modes, singular information and multiple dominant modes invalidate the single interior Gaussian formula; distinct nondegenerate dominant modes must have their contributions added.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
