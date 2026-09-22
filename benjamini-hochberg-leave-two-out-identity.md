# Benjamini-Hochberg leave-two-out identity

↑ **Parent:** [Benjamini-Hochberg leave-one-out identity](benjamini-hochberg-leave-one-out-identity.md)

Replace two [p-values](p-value.md) $P_i,P_j$ by zeros in the [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md) at level $\alpha$, keeping the original denominator $m$, and let $R^{(ij)}$ be the resulting rejection count. Equivalently, remove the two values and apply the step-up critical values $\alpha(k+2)/m$ to the remaining ordered [p-values](p-value.md); their rejection count is $R_{-ij}=R^{(ij)}-2$. For $r\ge2$,

$$
\{P_i\le\alpha r/m,\ P_j\le\alpha r/m,\ R=r\}
=\{P_i\le\alpha r/m,\ P_j\le\alpha r/m,\ R^{(ij)}=r\}.
$$

If both original values are rejected, lowering them changes no ordered rank greater than $r$, so the rejection count stays $r$. Conversely, if the modified count is $r$ and both original values meet the rank-$r$ threshold, reinserting them leaves at least $r$ qualifying values. Monotonicity under lowering gives at most $r$ original rejections. This identity is deterministic and does not require [independence](independent-random-variables.md) or a distributional assumption.

**Table of contents**

- [Second moment of the Benjamini-Hochberg false discovery proportion](second-moment-of-the-benjamini-hochberg-false-discovery-proportion.md)

## ↑ Ancestors (10)

1. [Benjamini-Hochberg leave-one-out identity](benjamini-hochberg-leave-one-out-identity.md)
2. [Benjamini-Hochberg procedure](benjamini-hochberg-procedure.md)
3. [Multiple hypothesis testing](multiple-hypothesis-testing.md)
4. [Statistical hypothesis test](statistical-hypothesis-test.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/4/solution.md)
- [Second moment of the Benjamini-Hochberg false discovery proportion](second-moment-of-the-benjamini-hochberg-false-discovery-proportion.md)
