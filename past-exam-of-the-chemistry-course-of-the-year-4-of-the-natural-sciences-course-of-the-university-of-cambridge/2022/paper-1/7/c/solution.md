<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The constant density is reasonable when the [integrand](../../../../../integrand.md) has comparable magnitude throughout the interval. It is inefficient for a narrow peak because most samples contribute little while rare samples carry large weights.

For independent [importance sampling](../../../../../importance-sampling.md),

$$
\operatorname{Var}(\widehat I_N)=\frac1N\left[\int_a^b\frac{f(x)^2}{q(x)}\,dx-I^2\right].
$$

A good density has support wherever $f\ne0$, is easy to sample and evaluate, and resembles $|f|$. Subject to normalization, **$q\propto|f|$ minimizes this [variance](../../../../../variance-split.md)**. For nonnegative $f$, the ideal normalized choice makes every sample contribution equal, although its normalization is generally the unknown integral itself. Uniform weighting is therefore acceptable for a flat [integrand](../../../../../integrand.md), not universally suitable.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
