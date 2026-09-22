<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Bartlett correction](../../../../../../bartlett-correction.md) improves calibration of a regular [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md) $W=2\{\ell(\widehat\theta)-\ell(\widehat\theta_0)\}$, whose null limit is $\chi_q^2$ for $q$ tested restrictions. If

$$
\mathbb E_0W=q\left(1+\frac bn+O(n^{-2})\right),
$$

the corrected statistic is $\boxed{W_B=W/(1+b/n)}$. Its null mean is $q+O(n^{-2})$ and it is compared with the same limiting [chi-squared distribution](../../../../../../chi-squared-distribution.md). The coefficient is model-specific, may involve nuisance parameters, and can be calculated from likelihood cumulants or a suitable null simulation; substitution must respect the asymptotic regime.

Under the regular higher-order likelihood expansions and identities that establish Bartlett correctability, this rescaling removes the leading $O(n^{-1})$ distributional error and can give $O(n^{-2})$ chi-square calibration error. Matching one moment by itself does not prove that assertion for an arbitrary statistic, and nonregular boundary or singular models need different treatment.

For illustration, testing a normal variance with unknown mean gives $W=n[-\log(U/n)+U/n-1]$ with $U\sim\chi_{n-1}^2$. The gamma logarithmic moment yields

$$
\mathbb E_0W=n\left[\log(n/2)-\operatorname{digamma}((n-1)/2)\right]-1=1+\frac{11}{6n}+O(n^{-2}).
$$

Thus the [Bartlett correction for a normal variance with unknown mean](../../../../../../bartlett-correction-for-a-normal-variance-with-unknown-mean.md) uses $b=11/6$, not the correction for the different known-mean model. This example also distinguishes the relative coefficient $b$ from the full divisor $1+b/n$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
