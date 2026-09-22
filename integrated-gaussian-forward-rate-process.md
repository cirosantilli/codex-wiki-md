# Integrated Gaussian forward-rate process

↑ **Parent:** [Gaussian forward-rate field](gaussian-forward-rate-field.md)

For a centered [Gaussian forward-rate field](gaussian-forward-rate-field.md) with covariance $\operatorname{Cov}(X(s,u),X(r,w))=c(s\wedge r,u,w)$, integrate the short-rate past and the current forward curve together using the displayed [mean-square integral](mean-square-integral.md). Its [variance](variance-split.md) is

$$
v(s,T)=\int_0^T\int_0^T c(s\wedge u\wedge w,u,w)\,du\,dw.
$$

For fixed $T$, its increments are independent of the full earlier forward-rate [filtration](filtration-probability-theory.md): their covariance with $X(z,w)$ at $z\leq r\leq s$ is the integral of $c(s\wedge u\wedge z,u,w)-c(r\wedge u\wedge z,u,w)=0$. Use the [uncorrelated jointly Gaussian variables are independent](uncorrelated-jointly-normal-variables-are-independent.md) principle first for finite collections and then for their generated [sigma-algebra](sigma-algebra.md). With $c(0,u,w)=0$, this centered process starts at zero.

**Table of contents**

- [Gaussian forward-rate covariance drift restriction](gaussian-forward-rate-covariance-drift-restriction.md)

## ↑ Ancestors (9)

1. [Gaussian forward-rate field](gaussian-forward-rate-field.md)
2. [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
3. [Interest rate](interest-rate.md)
4. [Fixed-income security](fixed-income-security.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Gaussian forward-rate covariance drift restriction](gaussian-forward-rate-covariance-drift-restriction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/solution.md)
