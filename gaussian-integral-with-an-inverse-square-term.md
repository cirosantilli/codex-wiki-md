# Gaussian integral with an inverse-square term

↑ **Parent:** [Gaussian integral](gaussian-integral.md)

For $a,b>0$, the integrand is even and integrable at zero and infinity. On the positive half-axis the [change of variables](change-of-variables-formula.md) $u=\sqrt a\,x-\sqrt b/x$ maps $(0,\infty)$ bijectively onto $\mathbb R$ and satisfies $ax^2+b/x^2=u^2+2\sqrt{ab}$. Solving the quadratic for the positive root gives

$$
\frac{dx}{du}=\frac1{2\sqrt a}\left(1+\frac u{\sqrt{u^2+4\sqrt{ab}}}\right).
$$

After doubling this half-axis integral, the odd part of the transformed integrand integrates to zero and the remaining [Gaussian integral](gaussian-integral.md) yields the formula. The reciprocal substitution $x=1/t$ also gives

$$
\int_{-\infty}^{\infty}x^{-2}e^{-(ax^2+b/x^2)/2}dx=\sqrt{2\pi/b}\,e^{-\sqrt{ab}}.
$$

The positive parameters ensure that the substitutions and improper integrals are valid; the second identity can also be recovered by differentiating the first in $b$ under the integral sign.

## ↑ Ancestors (8)

1. [Gaussian integral](gaussian-integral.md)
2. [Integral](integral-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/12/solution.md)
