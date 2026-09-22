# Inflow advection energy estimate from summation by parts

↑ **Parent:** [Discrete summation by parts](discrete-summation-by-parts.md)

For $U_t=-cDU$ with $c>0$, a positive discrete norm matrix $H$ satisfying the displayed identity gives $d(U^THU)/dt=-c(U_N^2-U_0^2)$. Homogeneous inflow data $U_0=0$ therefore leave only the nonpositive outflow flux. Inhomogeneous inflow contributes a controlled boundary forcing term. This estimate includes the numerical boundary closure, unlike an interior-only [Fourier stability analysis](fourier-stability-analysis.md). For any dissipative semidiscrete operator in the $H$ norm, [Backward Euler method](backward-euler-method.md) steps preserve the contraction by the identity $\|U^{n+1}\|_H^2-\|U^n\|_H^2=2k\langle U^{n+1},AU^{n+1}\rangle_H-\|U^{n+1}-U^n\|_H^2$.

## ↑ Ancestors (8)

1. [Discrete summation by parts](discrete-summation-by-parts.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/7/solution.md)
