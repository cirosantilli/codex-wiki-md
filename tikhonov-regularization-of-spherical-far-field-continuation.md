# Tikhonov regularization of spherical far-field continuation

↑ **Parent:** [Tikhonov regularization](tikhonov-regularization.md)

Let $d_n=ki^{n+1}h_n^{(1)}(kR)$ and map the near-field trace to the far field by $A g=(g_n^m/d_n)_{n,m}$. Quadratic [Tikhonov regularization](tikhonov-regularization.md) minimizes $\|Ag-y^\delta\|^2+\alpha\|g\|^2$ and yields the displayed filtered coefficients. Its data-error gain is at most $1/(2\sqrt\alpha)$. Total error also contains bias: $\|g_\alpha^\delta-g^\dagger\|\le\delta/(2\sqrt\alpha)+\|\alpha(A^*A+\alpha I)^{-1}g^\dagger\|$. A convergent parameter rule has $\alpha\to0$ and $\delta/\sqrt\alpha\to0$. Under $g^\dagger=A^*Aw$, $\|w\|\le C$, the bias is at most $C\alpha$; choosing $\alpha=(\delta/(4C))^{2/3}$ minimizes that error bound. Making $\alpha$ indefinitely large removes noise by shrinking the reconstruction to zero, not by recovering the true field.

## ↑ Ancestors (7)

1. [Tikhonov regularization](tikhonov-regularization.md)
2. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80/4/c/solution.md)
