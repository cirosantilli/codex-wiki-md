# Convolution theorem for Laplace transforms

↑ **Parent:** [Laplace transform](laplace-transform.md)

For [functions](function-split.md) $f,g$ on $[0,\infty)$ with $e^{-\sigma t}f(t)$ and $e^{-\sigma t}g(t)$ [Lebesgue integrable functions](lebesgue-integrable-function.md), their unilateral [convolution](convolution.md), defined [almost everywhere](almost-everywhere.md) if necessary, satisfies

$$
\mathcal L\{f*g\}(s)=F(s)G(s),\qquad (f*g)(t)=\int_0^tf(\tau)g(t-\tau)\,d\tau,\qquad \operatorname{Re}s=\sigma.
$$

Taking a [causal extension by zero](causal-extension-by-zero.md) of both [functions](function-split.md) gives the existing whole-line [convolution](convolution.md) definition. [Absolute convergence](absolute-convergence.md) and [Fubini's theorem](fubini-s-theorem.md) justify the product rule: put $t=\tau+u$ in the double [integral](integral-split.md), so $e^{-st}=e^{-s\tau}e^{-su}$. For [piecewise continuous functions](piecewise-continuous-function.md) of [exponential order](exponential-order.md) $a$ and $b$, the hypotheses hold for $\operatorname{Re}s>\max(a,b)$. The [Laplace transform](laplace-transform.md) article works out the concrete example $h(t)=e^{-2t}$ and the [Heaviside step function](heaviside-step-function.md) input, whose output is $(1-e^{-2t})/2$. [MIT 18.03SC, convolution and system response](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/0d4d90053f2bb24f7551c78e2d1b21a2_MIT18_03SCF11_s30_5text.pdf).

## ↑ Ancestors (6)

1. [Laplace transform](laplace-transform.md)
2. [Integral transform](integral-transform-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Abel integral equation of fractional order](abel-integral-equation-of-fractional-order.md)
- [Laplace transform](laplace-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/8a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/15f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/5/solution.md)
