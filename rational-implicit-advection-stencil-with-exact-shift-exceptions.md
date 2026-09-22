# Rational implicit advection stencil with exact shift exceptions

↑ **Parent:** [Finite difference method](finite-difference-method.md)

Consider a one-step stencil with new-level coefficients $a=\mu(1+\mu)/2$, $b=(1+\mu)(2-\mu)$ and $c=(1-\mu)(2-\mu)/2$ at offsets $-1,0,1$, and old-level coefficients $d=2-\mu$, $e=1+\mu$ at offsets $0,1$. For $u_t=u_x$, its exact-solution residual starts at fourth degree with coefficient $\mu(\mu-2)(\mu-1)(\mu+1)/24$. Thus its normalized [local truncation error](local-truncation-error.md) is third order at fixed nonzero [Courant number](courant-number.md), except at the exact-shift values $-1,1,2$; zero gives the zero-step identity. For its [Fourier symbol](fourier-symbol-of-a-difference-operator.md), $|D|^2-|N|^2=\mu(\mu-2)(\mu-1)(\mu+1)(1-\cos\theta)^2$. Uniformly invertible stable steps occur for $\mu\leq-1$, $0\leq\mu\leq1$ or $\mu\geq2$.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80/4/a/solution.md)
