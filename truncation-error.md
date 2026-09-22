# Truncation error

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Truncation_error)

[Truncation error](truncation-error.md) is introduced by replacing an exact operation with a finite approximation. It remains even when all arithmetic is exact. For $f(x)=x^2$, the forward [finite difference](finite-difference-split.md) for its [derivative](derivative.md) at $x=1$ gives

$$
\frac{f(1+h)-f(1)}h=2+h,\qquad f'(1)=2.
$$

Thus the [truncation error](truncation-error.md) is exactly $h$: $h=0.1$ gives $2.1$ and $h=0.01$ gives $2.01$. In finite precision, however, the numerator subtracts nearly equal values, and their [roundoff error](round-off-error.md) can be amplified by division by $h$. For smooth data with bounded evaluation errors of scale $u$, a typical bound has competing terms $C_1h+C_2u/h$. Smaller $h$ reduces the first term and increases the second; with fixed positive constants the balancing scale is $h\sim\sqrt u$. This is why blindly refining a [finite difference](finite-difference-split.md) eventually stops improving it.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Numerical analysis](numerical-analysis-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/39a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/5c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/5c/c/solution.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Round-off error](round-off-error.md)
- [Truncation error](truncation-error.md)
