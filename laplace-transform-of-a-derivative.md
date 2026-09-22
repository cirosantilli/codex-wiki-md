# Laplace transform of a derivative

↑ **Parent:** [Laplace transform](laplace-transform.md)

Suppose $f$ is an [absolutely continuous function](absolutely-continuous-function.md) on every finite [interval](interval-mathematics.md) $[0,T]$, both $e^{-st}f(t)$ and $e^{-st}f'(t)$ are [Lebesgue integrable functions](lebesgue-integrable-function.md), and $e^{-sT}f(T)\to0$. Then [integration by parts](integration-by-parts.md) on $[0,T]$ followed by a [limit](limit-of-a-function.md) gives

$$
\int_0^T e^{-st}f'(t)\,dt=e^{-sT}f(T)-f(0+)+s\int_0^Te^{-st}f(t)\,dt,\qquad \mathcal L\{f'\}(s)=sF(s)-f(0+).
$$

Here $f(0+)$ is the right [one-sided limit](one-sided-limit.md). [Exponential order](exponential-order.md) bounds on $f$ and $f'$ suffice when $\operatorname{Re}s$ exceeds both bounds. For $f(t)=e^{-2t}$, the identity reads $-2/(s+2)=s/(s+2)-1$ on $\operatorname{Re}s>-2$. This is the ordinary [derivative](derivative.md) on nonnegative time; differentiating a [causal extension by zero](causal-extension-by-zero.md) at its jump instead introduces a [Dirac delta function](dirac-delta-function.md). [MIT 18.03SC, derivative rules and initial data](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/22aba4126352ce0f76930d858d8dffa5_MIT18_03SCF11_s29_1text.pdf).

## ↑ Ancestors (6)

1. [Laplace transform](laplace-transform.md)
2. [Integral transform](integral-transform-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Laplace transform](laplace-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/15f/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/14a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/14a/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/12b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/5/i/solution.md)
