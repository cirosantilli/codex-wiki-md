# Periodic Gaussian process with zero period average

↑ **Parent:** [Periodic covariance function](periodic-covariance-function.md)

A zero-mean [Gaussian process](gaussian-process.md) need not have zero average in each realization. For the [periodic covariance function](periodic-covariance-function.md), the constant Fourier component is

$$
c_0=\frac1P\int_0^Pk_P(t,u)\,du=A^2e^{-\ell^{-2}}I_0(\ell^{-2}),
$$

where $I_0$ is a [modified Bessel function](modified-bessel-function.md). Replacing $f(t)$ by $f(t)-P^{-1}\int_0^Pf(u)\,du$ gives a Gaussian process with kernel $k_P(t,t')-c_0$. This is a [positive-semidefinite kernel](positive-semidefinite-kernel.md) because it is a covariance after a linear transformation, and each sample has zero period average. The [real integral representation of the modified Bessel function I0](real-integral-representation-of-the-modified-bessel-function-i0.md) yields the displayed constant.

## ↑ Ancestors (8)

1. [Periodic covariance function](periodic-covariance-function.md)
2. [Gaussian process](gaussian-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/3/ii/solution.md)
