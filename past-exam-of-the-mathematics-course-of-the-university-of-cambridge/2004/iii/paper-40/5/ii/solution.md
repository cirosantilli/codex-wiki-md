<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the standard interpretation that the counts are conditionally [independent](../../../../../../independent-random-variables.md) given the parameters, with mutually [independent](../../../../../../independent-random-variables.md) stated priors. Let $a_2=\alpha_2$, $b_2=\beta_2$, and define

$$
T=\sum_{i,j,t}x_{ijt},\qquad
R=\sum_{i,t}x_{i2t},\qquad
C=\sum_{i,j}x_{ij2},\qquad
E=I(1+e^{a_2})(1+e^{b_2}).
$$

Under the reference constraints, the [Poisson distribution](../../../../../../poisson-distribution.md) [likelihood](../../../../../../likelihood-function.md), up to data-only factors, is

$$
L(\theta,a_2,b_2)=\theta^T\exp\{Ra_2+Cb_2-\theta E\}.
$$

Multiplying by the shape-rate gamma prior gives the [Poisson-gamma conjugacy with unequal exposures](../../../../../../poisson-gamma-conjugacy-with-unequal-exposures.md)

$$
\boxed{\theta\mid a_2,b_2,\mathbf x
\sim\Gamma(a+T,b+I(1+e^{a_2})(1+e^{b_2})).}
$$

Here $b$ is a rate, matching the [probability density function](../../../../../../probability-density-function.md) convention on the PDF's first page. The factor $I$ represents the number of replicates per cell, not the total count.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
