# Fourier bounds for Schwartz functions

↑ **Parent:** [Fourier transform isomorphism of the Schwartz space](fourier-transform-isomorphism-of-the-schwartz-space.md)

For the angular-frequency [Fourier transform](fourier-transform-split.md) and [Schwartz seminorms](schwartz-seminorm.md) $p_{m,n}(\phi)=\sup_x|x^m\phi^{(n)}(x)|$, every output [seminorm](seminorm.md) is bounded by finitely many input [seminorms](seminorm.md). To prove this, [differentiation under the integral sign](differentiation-under-the-integral-sign.md) and [integration by parts](integration-by-parts.md) give

$$
\xi^m\partial_\xi^n\widehat\phi=i^{-m}\mathcal F\!\left[\partial_x^m((-ix)^n\phi)\right].
$$

The [generalized Leibniz rule](generalized-leibniz-rule.md), $\|\widehat g\|_\infty\leq\|g\|_1$, and $\|x^a\phi^{(b)}\|_1\leq\pi(p_{a,b}+p_{a+2,b})$ imply

$$
p_{m,n}(\widehat\phi)\leq\pi\sum_{j=0}^{\min(m,n)}\binom mj\frac{n!}{(n-j)!}
\bigl(p_{n-j,m-j}(\phi)+p_{n-j+2,m-j}(\phi)\bigr).
$$

This proves continuity of the [Fourier transform](fourier-transform-split.md) on the [Schwartz space](schwartz-space.md) and rapid decay of every transformed [derivative](derivative.md).

## ↑ Ancestors (6)

1. [Fourier transform isomorphism of the Schwartz space](fourier-transform-isomorphism-of-the-schwartz-space.md)
2. [Fourier transform](fourier-transform-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/1/a/i/solution.md)
- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/1/a/ii/solution.md)
- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/1/a/iii/solution.md)
- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/3/a/iii/solution.md)
