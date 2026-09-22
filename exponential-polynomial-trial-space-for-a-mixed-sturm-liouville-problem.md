# Exponential-polynomial trial space for a mixed Sturm-Liouville problem

↑ **Parent:** [Rayleigh-Ritz method](rayleigh-ritz-method.md)

For $-(p y')'=\lambda w y$ on $[0,1]$ with $p=(1+x)e^{2x}$, $w=e^{2x}$, $y(0)=0$ and $y'(1)=0$, the [Rayleigh quotient](rayleigh-quotient.md) is $\int p y'^2/\int w y^2$. The trial $y_1=xe^{-x}$ gives numerator $5/12$ and denominator $1/3$, hence $0<\lambda_{\min}\leq5/4$. Every displayed $y_n$ obeys the same mixed [boundary conditions](boundary-condition.md); so does $\sin[(m+1/2)\pi x]$. Adding any of these to the trial space cannot worsen the optimized upper bound. Matrix elements $A_{ij}=\int p y_i'y_j'$ and $M_{ij}=\int w y_iy_j$ give a finite-dimensional [generalized eigenvalue problem](generalized-eigenvalue-problem.md) $Av=\lambda Mv$. The case $n=1$ repeats the original trial and adds no variational freedom.

## ↑ Ancestors (7)

1. [Rayleigh-Ritz method](rayleigh-ritz-method.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/10/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/10/d/i/solution.md)
