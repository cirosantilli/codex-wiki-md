# Compact third-order advection stencil

↑ **Parent:** [Transport equation](transport-equation.md)

Let $a=\mu(1+\mu)/2$, $b=(1+\mu)(2-\mu)$, $c=(1-\mu)(2-\mu)/2$, $d=2-\mu$, and $e=1+\mu$. The implicit stencil $aU_{j-1}^{n+1}+bU_j^{n+1}+cU_{j+1}^{n+1}=dU_j^n+eU_{j+1}^n$ for $u_t=u_x$ has centered characteristic moments zero through degree three and fourth moment $K(\mu)$. Its Fourier numerator and denominator satisfy $|L(\theta)|^2-|N(\theta)|^2=K(\mu)(1-\cos\theta)^2$. The marching operator is a contraction exactly for nonnegative [Courant numbers](courant-number.md) in $[0,1]\cup[2,\infty)$; with signed Courant numbers, also include $(-\infty,-1]$. At the four roots of $K$ the method becomes an exact integer grid translation rather than merely third order.

## ↑ Ancestors (6)

1. [Transport equation](transport-equation.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/3/a/solution.md)
