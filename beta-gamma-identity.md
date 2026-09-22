# Beta-gamma identity

↑ **Parent:** [Beta function](beta-function.md)

For $p,q>0$, express the product of the two [Gamma integrals](gamma-integral.md) as the nonnegative [double integral](double-integral.md)

$$
\Gamma(p)\Gamma(q)=\int_0^\infty\int_0^\infty x^{p-1}y^{q-1}e^{-(x+y)}dx\,dy.
$$

Use $r=x+y$ and $u=x/(x+y)$, with inverse $x=ru$, $y=r(1-u)$ and [Jacobian determinant](jacobian-determinant.md) of absolute value $r$. The new [domain of integration](domain-of-integration.md) is $r>0$, $0<u<1$, and the integrand with this factor becomes $r^{p+q-1}e^{-r}u^{p-1}(1-u)^{q-1}$. [Tonelli's theorem](tonelli-theorem.md) and separation of the two integrals therefore give $\Gamma(p+q)B(p,q)$. The positive real parameter hypothesis ensures that all the original integrals are finite.

For complex parameters with positive real parts, the same proof first gives the undivided identity $\Gamma(p+q)B(p,q)=\Gamma(p)\Gamma(q)$. Absolute integrability follows by taking real parts in the exponents, so [Fubini's theorem](fubini-s-theorem.md) applies. The [nonvanishing of the Gamma function](gamma-function-has-no-zeros.md) then permits division by $\Gamma(p+q)$.

**Table of contents**

- [Sum-and-ratio substitution for gamma integrals](sum-and-ratio-substitution-for-gamma-integrals.md)

## ↑ Ancestors (7)

1. [Beta function](beta-function.md)
2. [Gamma function](gamma-function.md)
3. [Complex analysis](complex-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Abel integral equation of fractional order](abel-integral-equation-of-fractional-order.md)
- [Beta distribution](beta-distribution.md)
- [Beta-function recurrence](beta-function-recurrence.md)
- [Gamma function has no zeros](gamma-function-has-no-zeros.md)
- [Mellin integral of a reciprocal binomial](mellin-integral-of-a-reciprocal-binomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/14e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/7b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/7a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/16/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/5/solution.md)
