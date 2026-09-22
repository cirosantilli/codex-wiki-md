# Logarithmically smoothed Perron formula

↑ **Parent:** [Perron's formula](perron-s-formula.md)

If the [Dirichlet series](dirichlet-series.md) $F(s)=\sum_na_nn^{-s}$ is absolutely convergent at $\sigma>0$, then

$$
\sum_{n\le x}a_n\log(x/n)
=\frac1{2\pi i}\int_{\sigma-i\infty}^{\sigma+i\infty}\frac{F(s)x^s}{s^2}\,ds
=\frac1{2\pi}\int_{\mathbb R}\frac{F(\sigma+it)x^{\sigma+it}}{(\sigma+it)^2}\,dt.
$$

The scalar kernel is $(2\pi)^{-1}\int_{\mathbb R}e^{v(\sigma+it)}(\sigma+it)^{-2}dt=v_+$. This follows by [Fourier inversion](fourier-inversion-theorem.md) applied to $u e^{-\sigma u}\mathbf1_{u\ge0}$, whose [Fourier transform](fourier-transform.md) is $(\sigma+it)^{-2}$. Absolute convergence of the series and of $\int |\sigma+it|^{-2}dt$ justifies interchange. The factor $ds=i\,dt$ is essential.

**Table of contents**

- [Unsmoothing a logarithmically weighted sum](unsmoothing-a-logarithmically-weighted-sum.md)

## ↑ Ancestors (7)

1. [Perron's formula](perron-s-formula.md)
2. [Dirichlet series](dirichlet-series.md)
3. [Analytic number theory](analytic-number-theory-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/2/solution.md)
- [Unsmoothing a logarithmically weighted sum](unsmoothing-a-logarithmically-weighted-sum.md)
