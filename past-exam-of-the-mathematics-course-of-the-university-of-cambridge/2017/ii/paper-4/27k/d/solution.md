<h1 id="27k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the convention that the [likelihood ratio](../../../../../../likelihood-ratio.md) is maximized alternative likelihood divided by null likelihood. The alternative excludes zero, but its supremum agrees with the unrestricted maximum, even on the exceptional sample $\overline X=0$. [Completing the square](../../../../../../completing-the-square.md) gives

$$
\boxed{\Lambda(\Theta_1,\Theta_0)=\exp\left(\frac n2\|\overline X\|^2\right),\qquad2\log\Lambda=n\|\overline X\|^2.}
$$

Under the null, $\sqrt n\overline X\sim\mathcal N_d(0,I_d)$, so $2\log\Lambda\sim\chi_d^2$ exactly for every $n$. Equivalently $\Lambda$ is distributed as $e^{Y/2}$ for $Y\sim\chi_d^2$. With the reciprocal likelihood-ratio convention the statistic is $-2\log\Lambda$ instead.

[Wilks theorem](../../../../../../wilks-theorem.md) predicts a limiting [chi-squared distribution](../../../../../../chi-squared-distribution.md) with [degrees of freedom](../../../../../../degree-of-freedom.md) equal to the difference of parameter dimensions, here $d-0=d$, under regularity and an interior null point of the unrestricted model. This example strengthens the asymptotic conclusion to an exact finite-sample identity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [27K](../../27k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
