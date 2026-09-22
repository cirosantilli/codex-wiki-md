# Fourier sine series of an odd quadratic arch

↑ **Parent:** [Fourier sine series](fourier-sine-series.md)

Extend $F_L(x)=x(L-|x|)$ from $[-L,L]$ to a [periodic function](periodic-function.md) of period $2L$, with $L>0$. It is odd and continuous, so its [Fourier series](fourier-series-split.md) contains only sine terms. Its [Fourier coefficients](fourier-coefficient.md) are

$$
b_n=\frac2L\int_0^Lx(L-x)\sin(n\pi x/L)\,dx
=\frac{4L^2(1-(-1)^n)}{n^3\pi^3}.
$$

Two applications of [integration by parts](integration-by-parts.md) prove the coefficient formula. The first has no endpoint contribution because $x(L-x)$ vanishes at both endpoints; the second leaves a multiple of $1-\cos(n\pi)$. Thus only odd frequencies survive, giving the displayed [Fourier sine series](fourier-sine-series.md). Its absolutely summable coefficients give uniform convergence, and [Fourier orthogonality](fourier-orthogonality.md) identifies its sum with $F_L$.

Taking $L=1$, $\int_{-1}^1F_1(x)^2dx=2\int_0^1x^2(1-x)^2dx=1/15$. [Parseval's identity](parseval-identity.md) therefore gives

$$
\sum_{m=0}^\infty\frac1{(2m+1)^6}=\frac{\pi^6}{960}.
$$

## ↑ Ancestors (6)

1. [Fourier sine series](fourier-sine-series.md)
2. [Fourier series](fourier-series-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/17/c/solution.md)
