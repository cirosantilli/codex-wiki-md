# Periodic sine with an endpoint-correcting linear term

↑ **Parent:** [Periodic diffusion on a circle](periodic-diffusion-on-a-circle.md)

For $L>0$, extend $f_L(x)=\sin x-x\sin L/L$ from $[-L,L]$ periodically. The linear term makes both endpoint values zero and the endpoint first [derivatives](derivative.md) match. The function is [odd](odd-function.md), so its [Fourier series](fourier-series-split.md) has only sine terms, with the displayed [Fourier coefficients](fourier-coefficient.md). Indeed, for $k_n=n\pi/L\ne1$,

$$
\int_0^L\sin x\sin(k_nx)dx=\frac{(-1)^nk_n\sin L}{1-k_n^2},\qquad \int_0^Lx\sin(k_nx)dx=-\frac{L(-1)^n}{k_n};
$$

subtracting and multiplying by $2/L$ proves the formula. The coefficients decay as $O(n^{-3})$. At $L=m\pi$, the single coefficient $b_m$ has removable [limit](limit-of-a-function.md) $1$, with all others zero. Multiplying $b_n$ by $e^{-\kappa k_n^2t}$ solves the corresponding [heat equation](heat-equation.md) on the [circle](circle.md).

## ↑ Ancestors (8)

1. [Periodic diffusion on a circle](periodic-diffusion-on-a-circle.md)
2. [Heat equation](heat-equation.md)
3. [Diffusion equation](diffusion-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/2/ii/solution.md)
