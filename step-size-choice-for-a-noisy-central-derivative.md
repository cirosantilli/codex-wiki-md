# Step-size choice for a noisy central derivative

↑ **Parent:** [Sharp central-secant derivative error](sharp-central-secant-derivative-error.md)

Suppose $|f'''|\le M$ and each sampled value of $f$ has [absolute error](absolute-error.md) at most $\delta$. For a [central finite difference](central-finite-difference.md) with $h>0$, the [triangle inequality](triangle-inequality.md) and the [sharp central-secant derivative error](sharp-central-secant-derivative-error.md) give

$$
|\widetilde d-f'|\le\frac{Mh^2}{6}+\frac\delta h.
$$

For $M,\delta>0$, the [derivative](derivative.md) of this bound is $Mh/3-\delta/h^2$. It changes sign at $h_*=(3\delta/M)^{1/3}$, proving the unique minimum, of value $(3\delta)^{2/3}M^{1/3}/2$. This balance explains why reducing the step indefinitely amplifies sample [absolute error](absolute-error.md) even as [truncation error](truncation-error.md) decreases.

## ↑ Ancestors (9)

1. [Sharp central-secant derivative error](sharp-central-secant-derivative-error.md)
2. [Central finite difference](central-finite-difference.md)
3. [Finite difference method](finite-difference-method.md)
4. [Finite difference](finite-difference-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/continuous-mathematics/5/d/solution.md)
