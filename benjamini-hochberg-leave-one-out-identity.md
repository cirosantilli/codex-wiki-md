# Benjamini-Hochberg leave-one-out identity

↑ **Parent:** [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md)

Let $R$ be the number of rejections by the [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md) at level $\alpha$, and let $R_i$ be the rejection count after replacing $p_i$ by zero. Then $R_i\ge1$ and

$$
\frac{\mathbf1\{i\text{ rejected}\}}{R\vee1}=\frac{\mathbf1\{p_i\le\alpha R_i/m\}}{R_i}.
$$

If $i$ was rejected, lowering its [p-value](p-value.md) does not change any ordered [p-value](p-value.md) beyond rank $R$, so $R_i=R$. Conversely, if $p_i\le\alpha R_i/m$, the other $R_i-1$ rejected values together with $p_i$ satisfy the original threshold; monotonicity gives $R=R_i$. For a valid true-null [p-value](p-value.md) independent of the others, conditioning on $R_i$ bounds the expectation of the right side by $\alpha/m$. Summing over true nulls proves [false discovery rate](false-discovery-rate.md) at most $m_0\alpha/m$.

**Table of contents**

- [Benjamini-Hochberg leave-two-out identity](benjamini-hochberg-leave-two-out-identity.md)
  - [Second moment of the Benjamini-Hochberg false discovery proportion](second-moment-of-the-benjamini-hochberg-false-discovery-proportion.md)
- [Exact false discovery rate under independent null p-values](exact-false-discovery-rate-under-independent-null-p-values.md)

## ↑ Ancestors (9)

1. [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md)
2. [Multiple hypothesis testing](multiple-hypothesis-testing.md)
3. [Statistical hypothesis test](statistical-hypothesis-test.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Exact false discovery rate under independent null p-values](exact-false-discovery-rate-under-independent-null-p-values.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/3/solution.md)
- [Second moment of the Benjamini-Hochberg false discovery proportion](second-moment-of-the-benjamini-hochberg-false-discovery-proportion.md)
