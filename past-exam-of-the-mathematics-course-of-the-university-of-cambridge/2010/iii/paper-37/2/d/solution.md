<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $h(q)=1$ for $q=0,3,6$ and $h(9)=2$. The new [normal linear model](../../../../../../normal-linear-model.md) allows an age-by-policy [interaction](../../../../../../interaction-statistics.md):

$$
Y_{agpq}=\mu+\alpha_a+\delta_p+\kappa_{ap}+\gamma_g+\xi_{h(q)}+\varepsilon_{agpq},\qquad \varepsilon_{agpq}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The [corner-point constraints](../../../../../../corner-point-constraint.md) are $\alpha_{21}=\delta_{\mathrm{3rd}}=\gamma_F=\xi_1=0$ and $\kappa_{21,p}=\kappa_{a,\mathrm{3rd}}=0$. Compared with the six-parameter reduced additive model, there are two additional interaction coefficients. Its [F-test](../../../../../../f-test.md) gives

$$
\boxed{F=\frac{(22323-10028)/2}{10028/24}=14.7128,\qquad p\simeq6.75\times10^{-5}.}
$$

Thus the interaction model significantly improves the reduced additive model. Estimated premiums decrease with age. Men have an estimated premium $94.375$ higher than women at fixed other characteristics, and 9 points adds $41.708$ relative to 0, 3, or 6. Comprehensive cover costs more than third-party cover, but its increment depends on age: $175.375$ at 21, $148.500$ at 30, and $79.500$ at 40. These are model-based comparisons, including extrapolations into the unobserved age-gender combinations.

For a 40-year-old woman with comprehensive cover and 6 points, the gender and points contrasts vanish. The fitted premium is

$$
\boxed{269.760-207.812+175.375-95.875=141.448.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
