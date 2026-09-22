# Fourier series of a half-wave rectified sinusoid

↑ **Parent:** [Fourier series](fourier-series-split.md)

For $V(t)=V_0\max(\sin\omega t,0)$, with period $2\pi/\omega$, [half-wave rectification](half-wave-rectifier.md) gives

$$
V(t)=\frac{V_0}{\pi}+\frac{V_0}{2}\sin\omega t
-\frac{2V_0}{\pi}\sum_{m=1}^\infty\frac{\cos(2m\omega t)}{4m^2-1}.
$$

The [Fourier coefficients](fourier-coefficient.md) are $a_0=2V_0/\pi$, $b_1=V_0/2$, $a_{2m}=-2V_0/[\pi(4m^2-1)]$, with all remaining coefficients zero. To derive the cosine coefficients, integrate $\sin s\cos ns$ over $0<s<\pi$ and use the product-to-sum identity. The sine coefficients follow from [orthogonality](orthogonal-vectors.md). A half-period delay reverses only the fundamental sine term and leaves the constant and even-frequency cosine terms unchanged, by [translation of a Fourier series](translation-of-a-fourier-series.md).

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/18/c/solution.md)
