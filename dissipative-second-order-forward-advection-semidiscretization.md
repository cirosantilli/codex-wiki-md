# Dissipative second-order forward advection semidiscretization

↑ **Parent:** [Method of lines](method-of-lines.md)

For periodic indexing let $S$ be the unitary forward shift. The operator is $A=-3I/2+2S-S^2/2$. A [discrete Fourier transform](discrete-fourier-transform.md) diagonalizes it with eigenvalue $\lambda(\theta)=-3/2+2e^{i\theta}-e^{2i\theta}/2$ and real part $-(1-\cos\theta)^2$. Consequently $\|e^{tA/h}\|_2\le1$ for every $t\ge0$, uniformly in the grid. Equivalently $A+A^*=-\tfrac12(2I-S-S^*)^2$, proving decay of the discrete energy directly. The result is semidiscrete [stability](stability-of-a-numerical-method.md); a further time discretization must also have adequate [absolute stability](linear-stability-domain.md).

## ↑ Ancestors (8)

1. [Method of lines](method-of-lines.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/5/solution.md)
