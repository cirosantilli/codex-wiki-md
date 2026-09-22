<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The null hypothesis is

$$
H_0:\beta_{\rm type2}=\beta_{\rm type3}
=\beta_{\rm posout}=0,
$$

against the alternative that at least one coefficient is nonzero. The code uses the scaled reduction in [exponential-family deviance](../../../../../../exponential-family-deviance.md),

$$
T=\frac{21.061-18.185}{0.31},
$$

and compares it with $\chi_3^2$.

That chi-squared calibration is appropriate when the dispersion is known, and is asymptotically valid after consistent dispersion estimation. With unknown Gamma dispersion, the standard finite-sample GLM comparison instead uses

$$
F=\frac{(21.061-18.185)/3}{0.3103711}
$$

against an $F_{3,57}$ distribution. Its p-value is approximately $0.034$, so the correctly calibrated test still rejects at the 5% level and gives evidence that component type or position contributes to mean failure time.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
