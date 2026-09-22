# Finite geometric series

↑ **Parent:** [Geometric series](geometric-series.md)

A finite geometric series is a [sum](sum.md) of consecutive terms of a [geometric progression](geometric-progression.md). With first term $a$ and $N$ terms, including $N=0$ for the empty sum,

$$
\boxed{S_N=\sum_{j=0}^{N-1}ar^j=
\begin{cases}
a(1-r^N)/(1-r),&r\ne1,\\
Na,&r=1.
\end{cases}}
$$

Unlike an infinite [geometric series](geometric-series.md), this identity does not need $|r|<1$. For example, $3+6+12+24+48=3(2^5-1)=93$. The number of terms is five; the largest exponent is four.

The cancellation behind the formula is especially useful to remember: multiplying $S_N$ by the [common ratio](common-ratio.md) shifts all terms one place. In $S_N-rS_N$, every interior term cancels, leaving $a-ar^N$. Division by $1-r$ gives the identity when $r\ne1$; at $r=1$ the sum is directly $Na$. The same argument works for [complex numbers](complex-number.md).

For integers $m\le n$ and $r\ne1$, the shifted version is

$$
\sum_{j=m}^n r^j=r^m\frac{1-r^{n-m+1}}{1-r}.
$$

There are $n-m+1$ terms. All powers must be defined; if a negative exponent is present, $r$ must be nonzero. At $r=1$ this sum is simply $n-m+1$. The [finite trigonometric sum](finite-trigonometric-sum.md) uses this identity with a [complex exponential](complex-exponential-function.md) as the [common ratio](common-ratio.md).

Finite sums of [positive integers](positive-integer.md) in a [geometric progression](geometric-progression.md) already appear in [Euclid's Elements](euclid-s-elements.md), Book IX, Proposition 35. The argument there compares differences of proportional numbers; Joyce's guide rewrites its conclusion as the modern finite-sum formula. This historical result concerns finite sums, without asserting an infinite [limit](limit-of-a-function.md). [Euclid, Elements IX.35, with David Joyce's guide to the algebraic form](https://mathcs.clarku.edu/~djoyce/elements/bookIX/propIX35.html)

**Table of contents**

- [Finite trigonometric sum](finite-trigonometric-sum.md)
- [Exponential geometric sum bound](exponential-geometric-sum-bound.md)

## ↑ Ancestors (7)

1. [Geometric series](geometric-series.md)
2. [Sequence and series](sequence-and-series.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Discrete-logarithm Fourier sampling](discrete-logarithm-fourier-sampling.md)
- [Finite trigonometric sum](finite-trigonometric-sum.md)
- [Geometric series](geometric-series.md)
- [Near-grid quantum phase estimation](near-grid-quantum-phase-estimation.md)
- [Nearest-integer success bound for quantum phase estimation](nearest-integer-success-bound-for-quantum-phase-estimation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/7/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-87/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/1b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/1b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/11i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/10c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/1/b/iii/solution.md)
- [Quadratic exponential sum](quadratic-exponential-sum.md)
- [Repdigit](repdigit.md)
- [Sum-of-divisors function](sum-of-divisors-function.md)
- [Universal lossless shortening is impossible](universal-lossless-shortening-is-impossible.md)
