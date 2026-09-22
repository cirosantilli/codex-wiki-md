# Centered two-step discretization of exponential decay

↑ **Parent:** [Parasitic amplification root](parasitic-amplification-root.md)

Replacing the derivative in $x'=-Kx$ by a [central finite difference](central-finite-difference.md) gives $x_{n+1}+2Khx_n-x_{n-1}=0$. Its principal root is $\rho_+=e^{-\operatorname{arsinh}(Kh)}$, while the [parasitic amplification root](parasitic-amplification-root.md) is $\rho_-=-e^{\operatorname{arsinh}(Kh)}$. On a fixed time interval, $A_h\rho_+^n+B_h\rho_-^n$ converges uniformly to $Ce^{-Kt}$ exactly when $A_h\to C$ and $B_h\to0$. A fixed nonzero parasitic amplitude alternates between two incompatible limits, but a vanishing starting error can converge despite the root's modulus exceeding one. This distinguishes fixed-time [numerical convergence](convergence-of-a-numerical-method.md) from long-time [absolute stability](linear-stability-domain.md).

## ↑ Ancestors (9)

1. [Parasitic amplification root](parasitic-amplification-root.md)
2. [Root condition for a multistep method](root-condition-for-a-multistep-method.md)
3. [Zero-stability](zero-stability.md)
4. [Linear multistep method](linear-multistep-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/2d/solution.md)
