# Second moment of the Benjamini-Hochberg false discovery proportion

↑ **Parent:** [Benjamini-Hochberg leave-two-out identity](benjamini-hochberg-leave-two-out-identity.md)

For independent [p-values](p-value.md), with $m_0$ true-null values independent and uniform on $[0,1]$, let $R^{(i)}$ denote the [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md) rejection count after replacing one true-null value by zero. The [Benjamini-Hochberg leave-one-out identity](benjamini-hochberg-leave-one-out-identity.md) gives

$$
\mathbb E\frac{\mathbf1\{i\text{ rejected}\}}{(R\vee1)^2}=\frac\alpha m\mathbb E\frac1{R^{(i)}}.
$$

For distinct true-null indices, the [Benjamini-Hochberg leave-two-out identity](benjamini-hochberg-leave-two-out-identity.md) gives

$$
\mathbb E\frac{\mathbf1\{i,j\text{ rejected}\}}{(R\vee1)^2}=\frac{\alpha^2}{m^2}.
$$

Indeed, conditional on the remaining values and $R^{(ij)}=r$, the two independent uniform values both meet their threshold with probability $(\alpha r/m)^2$, cancelling the denominator $r^2$. Expanding the square of the false rejection count into its diagonal terms and ordered distinct pairs, and using symmetry among the true-null values, proves

$$
\mathbb E(\operatorname{FDP}^2)=\frac{\alpha m_0}{m}\mathbb E\frac1{R^{(i)}}+\frac{\alpha^2m_0(m_0-1)}{m^2}.
$$

If no null is true, both sides are zero; if exactly one is true, the pair contribution is absent. This formula complements the exact [false discovery rate](false-discovery-rate.md) $\alpha m_0/m$ by describing second-moment variability.

## ↑ Ancestors (11)

1. [Benjamini-Hochberg leave-two-out identity](benjamini-hochberg-leave-two-out-identity.md)
2. [Benjamini-Hochberg leave-one-out identity](benjamini-hochberg-leave-one-out-identity.md)
3. [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md)
4. [Multiple hypothesis testing](multiple-hypothesis-testing.md)
5. [Statistical hypothesis test](statistical-hypothesis-test.md)
6. [Statistical modelling](statistical-modelling-split.md)
7. [Statistical model](statistical-model-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/4/solution.md)
