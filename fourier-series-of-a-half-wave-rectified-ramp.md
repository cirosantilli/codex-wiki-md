# Fourier series of a half-wave rectified ramp

↑ **Parent:** [Fourier series](fourier-series-split.md)

Extend $f(x)=\max(0,2x)$ on $(-1,1)$ with period two. Its [Fourier coefficients](fourier-coefficient.md) in the basis $\cos(n\pi x),\sin(n\pi x)$ are $a_0=1$, $a_n=2[(-1)^n-1]/(n\pi)^2$, and $b_n=2(-1)^{n+1}/(n\pi)$, by [integration by parts](integration-by-parts.md) on $(0,1)$. Thus

$$
f(x)\sim\frac12-\frac4{\pi^2}\sum_{r=0}^{\infty}\frac{\cos((2r+1)\pi x)}{(2r+1)^2}+\frac2\pi\sum_{n=1}^{\infty}\frac{(-1)^{n+1}\sin(n\pi x)}n.
$$

Its [even](even-function.md) part is the periodic extension of $|x|$ and its [odd](odd-function.md) part is the [Fourier series of a periodic sawtooth](fourier-series-of-a-periodic-sawtooth.md) for $x$. The cosine terms converge absolutely and uniformly; the sine terms account for the jump at odd integers. At each jump, the full [Fourier series](fourier-series-split.md) has value $1$, the average of the two one-sided limits $0$ and $2$.

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-b/8/solution.md)
