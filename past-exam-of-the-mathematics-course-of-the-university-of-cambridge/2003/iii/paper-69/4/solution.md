<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Periodicity and the [Hölder condition](../../../../../holder-condition.md) give $|f(x-t)-f(x)|\le M|t|^\alpha$ for $|t|\le\pi$. The positive normalized [Fejér kernel](../../../../../fejer-kernel.md) therefore yields

$$
\|\sigma_{n-1}f-f\|_\infty\le\frac{2M}{\pi}\int_0^\pi t^\alpha F_{n-1}(t)\,dt.
$$

The exponential-sum representation of the kernel bounds $F_{n-1}(t)\le n/2$. Also $\sin(t/2)\ge t/\pi$ for $0\le t\le\pi$, so $F_{n-1}(t)\le\pi^2/(2nt^2)$. Splitting at $1/n$ and using $0<\alpha<1$ gives

$$
\begin{aligned}
\int_0^\pi t^\alpha F_{n-1}(t)\,dt&\le\frac n2\int_0^{1/n}t^\alpha\,dt+\frac{\pi^2}{2n}\int_{1/n}^\pi t^{\alpha-2}\,dt\\
&\le\left(\frac1{2(\alpha+1)}+\frac{\pi^2}{2(1-\alpha)}\right)n^{-\alpha}.
\end{aligned}
$$

Hence the [Hölder error bound for Fejér summation](../../../../../holder-error-bound-for-fejer-summation.md) is

$$
\boxed{\|\sigma_{n-1}f-f\|_\infty\le M\left(\frac1{\pi(\alpha+1)}+\frac\pi{1-\alpha}\right)n^{-\alpha}.}
$$

The constant depends on the [Hölder exponent](../../../../../holder-exponent.md) and $M$, but not on $n$ or $f$ beyond its [Hölder seminorm](../../../../../holder-seminorm.md) bound.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
