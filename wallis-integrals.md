# Wallis integrals

↑ **Parent:** [Integral](integral.md)

The [Wallis integrals](wallis-integrals.md) are $I_n=\int_0^{\pi/2}\sin^n x\,dx$ for integers $n\geq0$. [Integration by parts](integration-by-parts.md) gives $nI_n=(n-1)I_{n-2}$ for $n\geq2$, with $I_0=\pi/2$, $I_1=1$. Hence

$$
I_{2n}=\frac{(2n)!}{2^{2n}(n!)^2}\frac\pi2,\qquad
I_{2n+1}=\frac{2^{2n}(n!)^2}{(2n+1)!}.
$$

Because $0<\sin x<1$ in the integration interval, $0<I_n<I_{n-1}$ for $n\geq1$. Combining this with the recurrence gives $2n/(2n+1)<I_{2n+1}/I_{2n}<1$, proving that the ratio tends to one and yielding the [Wallis product](wallis-product.md).

## ↑ Ancestors (7)

1. [Integral](integral.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/10e/solution.md)
- [Wallis integrals](wallis-integrals.md)
- [Wallis product](wallis-product.md)
