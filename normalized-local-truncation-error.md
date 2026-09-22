# Normalized local truncation error

↑ **Parent:** [Local truncation error](local-truncation-error.md)

For a time update with one-step defect $\delta_{h,k}$ after exact solution values are inserted, the normalized defect divides by the time step $k$. If $\delta_{h,k}=O(k^{p+1})$, the normalized [local truncation error](local-truncation-error.md) is $O(k^p)$. A spatial mesh contributes its own powers: for a diffusion update, $\mathcal T_{h,k}=O(k+h^2)$ means $\delta_{h,k}=O(k^2+kh^2)$. Under $k=O(h^2)$ these are respectively second and fourth powers of $h$. Neither normalization changes the actual [order of a numerical method](order-of-a-numerical-method.md); it changes the power used to express its residual.

## ↑ Ancestors (8)

1. [Local truncation error](local-truncation-error.md)
2. [Order of a numerical method](order-of-a-numerical-method.md)
3. [Consistency of a numerical method](consistency-of-a-numerical-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/2/a/solution.md)
