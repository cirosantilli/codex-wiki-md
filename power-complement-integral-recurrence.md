# Power-complement integral recurrence

↑ **Parent:** [Beta function](beta-function.md)

For $p>0$ and a nonnegative integer $n$, [integration by parts](integration-by-parts.md) gives, when $n>0$,

$$
J_n(p)=pn\int_0^1s^p(1-s^p)^{n-1}\,ds
=pn\bigl(J_{n-1}(p)-J_n(p)\bigr).
$$

The endpoint term $[s(1-s^p)^n]_0^1$ vanishes. Therefore

$$
J_n(p)=\frac{pn}{pn+1}J_{n-1}(p),\qquad J_0(p)=1.
$$

Repeated application yields $J_n(p)=\prod_{j=1}^n pj/(pj+1)$. The [integration by substitution](integration-by-substitution.md) $w=s^p$ also identifies $J_n(p)=B(1/p,n+1)/p$ with an [Euler beta function](beta-function.md). A related weighted [integral](integral-split.md) follows immediately from the same substitution:

$$
\int_0^1s^{p-1}(1-s^p)^n\,ds=\frac1{p(n+1)}.
$$

## ↑ Ancestors (7)

1. [Beta function](beta-function.md)
2. [Gamma function](gamma-function.md)
3. [Complex analysis](complex-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/12/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/12/c/solution.md)
