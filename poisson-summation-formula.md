# Poisson summation formula

↑ **Parent:** [Fourier analysis](fourier-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_summation_formula)

The [Poisson summation formula](poisson-summation-formula.md) equates sample sums of a [function](function-split.md) and its [Fourier transform](fourier-transform-split.md). Exchanging broad and narrow sums can save work. Use the convention

$$
\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-2\pi i\xi x}\,dx.
$$

For every [Schwartz function](schwartz-function.md) $f\in\mathcal S(\mathbb R)$,

$$
\boxed{\sum_{n\in\mathbb Z}f(n)=\sum_{k\in\mathbb Z}\widehat f(k).}
$$

Both [series](series-mathematics.md) have [absolute convergence](absolute-convergence.md). A sufficient hypothesis is that $f$ is [smooth](smooth-function.md) and $\sup_x(1+|x|)^M|f^{(r)}(x)|<\infty$ for all nonnegative [integers](integer-split.md) $M,r$; its [Fourier transform](fourier-transform-split.md) is then also a [Schwartz function](schwartz-function.md).[§3, Definition 32 and Exercise 54: Schwartz hypotheses and Poisson summation on the integer lattice](245c-notes-2-the-fourier-transform-by-terence-tao.md) This assumption controls both decay and regularity; mere membership of an [L1 space](l1-space.md) does not control values at individual sampling points, as [periodization of an integrable function](periodization-of-an-integrable-function.md) illustrates.

Here $\xi$ counts cycles per unit length. In the angular convention used elsewhere in [Fourier analysis](fourier-analysis-split.md), $\widetilde f(\omega)=\int f(x)e^{-i\omega x}\,dx$, so $\widehat f(\xi)=\widetilde f(2\pi\xi)$ and the right-hand side becomes $\sum_k\widetilde f(2\pi k)$. Keeping the [Fourier transform](fourier-transform-split.md) convention explicit prevents stray $2\pi$ factors. Changing the sample spacing leads to the [Poisson summation formula for a Euclidean lattice](poisson-summation-formula-for-a-euclidean-lattice.md).

**Table of contents**

- [Gaussian Poisson summation identity](gaussian-poisson-summation-identity.md)
  - [Gaussian sum truncation bound](gaussian-sum-truncation-bound.md)
- [Periodization of an integrable function](periodization-of-an-integrable-function.md)
- [Periodization of a Schwartz function](periodization-of-a-schwartz-function.md)
- [Poisson summation formula for a Euclidean lattice](poisson-summation-formula-for-a-euclidean-lattice.md)

## ↑ Ancestors (5)

1. [Fourier analysis](fourier-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Dual integer-height representation of the planar Villain model](dual-integer-height-representation-of-the-planar-villain-model.md)
- [Gaussian Poisson summation identity](gaussian-poisson-summation-identity.md)
- [Mellin representation of the completed Riemann zeta function](mellin-representation-of-the-completed-riemann-zeta-function.md)
- [Momentum-winding duality of a quantum rotor](momentum-winding-duality-of-a-quantum-rotor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/16e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-88/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/16a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-50/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-50/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-46/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-23/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-81/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/34a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-150/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-304/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-137/3/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2012/paper-1/3/d/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2016/paper-1/3/d/solution.md)
- [Periodization of a Schwartz function](periodization-of-a-schwartz-function.md)
- [Periodization of an integrable function](periodization-of-an-integrable-function.md)
- [Poisson summation formula](poisson-summation-formula.md)
- [Poisson summation formula for a Euclidean lattice](poisson-summation-formula-for-a-euclidean-lattice.md)
- [Real-time winding representation of a quantum rotor kernel](real-time-winding-representation-of-a-quantum-rotor-kernel.md)
- [Thermal trace of an interval image kernel](thermal-trace-of-an-interval-image-kernel.md)
- [Theta series of integer squares](theta-series-of-integer-squares.md)
- [Villain model](villain-model.md)
