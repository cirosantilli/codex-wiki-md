# Dini test for Fourier series

↑ **Parent:** [Fourier series](fourier-series-split.md)

For an integrable periodic function with one-sided limits $L_+,L_-$ at $t$, the displayed condition implies that its classical [Fourier partial sums](fourier-partial-sum.md) converge to $(L_++L_-)/2$. To prove it use the [Dirichlet kernel](dirichlet-kernel.md) $D_n(s)=\sin((n+1/2)s)/\sin(s/2)$ and its integral $2\pi$. Subtract the target value and combine the positive and negative halves of the convolution integral. The resulting difference is

$$
\frac1{2\pi}\int_0^\pi\frac{f(t+s)+f(t-s)-L_+-L_-}{\sin(s/2)}\sin((n+1/2)s)ds.
$$

The coefficient of the sine is integrable near zero by the Dini condition, and away from zero by integrability of $f$. The [Riemann-Lebesgue lemma](riemann-lebesgue-lemma.md) therefore makes this expression tend to zero. [Step functions](step-function.md) satisfy the condition because the numerator vanishes in a sufficiently small punctured neighborhood. This is a local Fourier convergence test, distinct from [Dini's theorem](dini-s-theorem.md) on uniform convergence of monotone sequences of [continuous functions](continuous-function.md).

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-analysis-course-of-the-university-of-oxford/2007/b/7/solution.md)
