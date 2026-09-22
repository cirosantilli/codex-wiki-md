<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Before introduction there is no local infection exposure. Let $H=2024-2005=19$ years, using the actual elapsed time between introduction and sampling if exact dates are available. A lifelong resident aged $a_i$ has therefore had only

$$
e_i=\min(a_i,H)
$$

years of possible exposure. With a constant post-introduction [force of infection](../../../../../force-of-infection.md) $\lambda$, replace age by this exposure duration:

$$
\boxed{p_i=1-e^{-\lambda\min(a_i,19)},\qquad\operatorname{cloglog}(p_i)=\beta_0+\ln\min(a_i,19)}.
$$

Fit the same [binomial regression](../../../../../binomial-regression.md) with $\ln e_i$ as its [offset](../../../../../generalized-linear-model-offset.md). The predicted [seroprevalence](../../../../../seroprevalence.md) increases with age up to 19 and then reaches a plateau, since older residents all began local exposure at introduction.

This is equivalent to using a calendar-time [force of infection](../../../../../force-of-infection.md) of zero before 2005 and $\lambda$ afterwards. With a changing post-introduction rate, the more general exposure is $\int_{\max(2005,\,2024-a_i)}^{2024}\lambda(u)\,du$. Account separately for migration or infection acquired elsewhere, since current residence alone need not specify lifetime exposure. Subjects with exactly zero exposure have model probability zero and cannot be included by taking $\ln0$ as an ordinary finite [offset](../../../../../generalized-linear-model-offset.md); handle them through the original probability model.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
