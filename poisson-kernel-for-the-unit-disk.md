# Poisson kernel for the unit disk

↑ **Parent:** [Laplace equation](laplace-equation.md)

For $0\le r<1$, this [Poisson kernel for the unit disk](poisson-kernel-for-the-unit-disk.md) has the uniformly convergent [Fourier series](fourier-series-split.md)

$$
P_r(\theta)=1+2\sum_{n=1}^\infty r^n\cos(n\theta).
$$

The identity follows by taking the [real part](real-part.md) of the [geometric series](geometric-series.md) $1+2\sum_{n\ge1}(re^{i\theta})^n$. For integrable $2\pi$-periodic boundary data $f$, its Poisson extension is

$$
u(r,\theta)=\frac1{2\pi}\int_{-\pi}^{\pi}P_r(\theta-t)f(t)\,dt
=\frac{a_0}{2}+\sum_{n=1}^\infty r^n[a_n\cos(n\theta)+b_n\sin(n\theta)],
$$

where $a_n,b_n$ are the usual [Fourier coefficients](fourier-coefficient.md). Each term is a [harmonic function](harmonic-function.md) in the open [disk](disk-mathematics.md). For continuous boundary data, the extension solves the [Dirichlet problem](dirichlet-problem.md) with those boundary values.

**Table of contents**

- [Disk potential with two semicircular boundary values](disk-potential-with-two-semicircular-boundary-values.md)
- [Area norm of the Poisson extension in the unit disk](area-norm-of-the-poisson-extension-in-the-unit-disk.md)

## ↑ Ancestors (7)

1. [Laplace equation](laplace-equation.md)
2. [Laplace operator](laplace-operator.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Area norm of the Poisson extension in the unit disk](area-norm-of-the-poisson-extension-in-the-unit-disk.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/18/b/solution.md)
- [Poisson kernel for the unit disk](poisson-kernel-for-the-unit-disk.md)
