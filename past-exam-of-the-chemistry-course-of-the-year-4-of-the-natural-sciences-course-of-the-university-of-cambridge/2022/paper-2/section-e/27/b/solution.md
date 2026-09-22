<h1 id="section-e/27/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The observed statistic is the **conditional mean among passages completed before $T=t_{\rm obs}$**, not a mean in which unfinished trajectories are assigned duration $T$. Its normalization is

$$
Z_T=\int_0^Tp(t)\,dt=\sum_lA_l(1-e^{-\nu_lT}).
$$

For each contribution,

$$
\int_0^Tt\nu_le^{-\nu_lt}dt=\left[-te^{-\nu_lt}\right]_0^T+\frac{1-e^{-\nu_lT}}{\nu_l}=\frac{1-e^{-\nu_lT}(1+\nu_lT)}{\nu_l}.
$$

Dividing the weighted sum of these first moments by $Z_T$ gives

$$
\boxed{\mathcal T(T)=\frac{\sum_l(A_l/\nu_l)[1-e^{-\nu_lT}(1+\nu_lT)]}{\sum_lA_l(1-e^{-\nu_lT})}.}
$$

The denominator records the fraction of trajectories actually observed to finish.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [27](../../27.md)
3. [Section E](../../../section-e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
