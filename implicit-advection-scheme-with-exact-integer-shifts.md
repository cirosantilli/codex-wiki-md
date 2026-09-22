# Implicit advection scheme with exact integer shifts

↑ **Parent:** [Finite difference method](finite-difference-method.md)

A three-point implicit advection stencil can match translated data through cubic [Taylor expansion](taylor-expansion.md) while retaining a rational [Fourier amplification symbol](fourier-amplification-symbol.md). For the coefficient family $a=\mu(1+\mu)/6$, $b=(2-\mu)(1+\mu)/3$, $c=(2-\mu)(1-\mu)/6$, $d=(2-\mu)/3$, $e=(1+\mu)/3$, its factor is $G=(d+e e^{i\theta})/(a e^{-i\theta}+b+c e^{i\theta})$. Direct subtraction gives $|D|^2-|N|^2=\mu(\mu-2)(\mu-1)(\mu+1)(1-\cos\theta)^2/9$. The displayed ranges are the contraction ranges in the [discrete L2 norm](discrete-l2-norm.md), with a nonvanishing denominator there. For forward time and positive speed parameter, retain the nonnegative ranges. For fixed nonzero nonexceptional [Courant number](courant-number.md), the normalized truncation error is third order; at $\mu=-1,0,1,2$ the update is the corresponding exact grid translation.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/3/a/solution.md)
