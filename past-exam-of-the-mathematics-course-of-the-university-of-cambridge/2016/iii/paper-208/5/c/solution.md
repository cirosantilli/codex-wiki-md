<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On $x>0$, the exponential proposal is the proper density $g(x)=e^{-x}\mathbf1_{\{x>0\}}$; its integral is $1$. The word “improper” in the question is therefore not applicable on its stated positive support.

The target-to-proposal ratio is

$$
\frac{f(x)}{g(x)}=\sqrt{\frac2\pi}\exp(-x^2/2+x)
=\sqrt{\frac{2e}{\pi}}\exp\left[-\frac{(x-1)^2}{2}\right].
$$

Its maximum occurs at $x=1$, so the smallest valid envelope constant is

$$
\boxed{M=\sqrt{2e/\pi},\qquad P(\mathrm{accept})=1/M=\sqrt{\pi/(2e)}\approx0.76017>0.75.}
$$

One implementation draws $Z=-\log U_1$ and accepts it when $U_2\leq e^{-(Z-1)^2/2}$, for [independent random variables](../../../../../../independent-random-variables.md) with the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$. Accepted observations have the positive half-normal density by the usual [rejection sampling](../../../../../../rejection-sampling.md) calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
