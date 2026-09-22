# Conjugate gradient convergence bound

↑ **Parent:** [Conjugate gradient method](conjugate-gradient-method.md)

For a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $H$, the [Conjugate gradient method](conjugate-gradient-method.md) minimizes the error in the induced [weighted norm](weighted-norm.md) over its affine [Krylov subspace](krylov-subspace.md). Writing the error as $p(H)e_0$ gives

$$
\frac{\|e_k\|_H}{\|e_0\|_H}\leq\min_{\deg p\leq k,\ p(0)=1}\max_{\lambda\in[\lambda_{\min},\lambda_{\max}]}|p(\lambda)|.
$$

For $\lambda_{\min}<\lambda_{\max}$, choose the scaled [Chebyshev polynomial](chebyshev-polynomial.md) $p(\lambda)=T_k((\lambda_{\max}+\lambda_{\min}-2\lambda)/(\lambda_{\max}-\lambda_{\min}))/T_k((\lambda_{\max}+\lambda_{\min})/(\lambda_{\max}-\lambda_{\min}))$. On the spectral interval its numerator has absolute value at most one. With $\rho=(\sqrt\kappa+1)/(\sqrt\kappa-1)$, the denominator equals $(\rho^k+\rho^{-k})/2\geq\rho^k/2$. This proves the displayed bound. If the two endpoints coincide, $H$ is a positive scalar multiple of the identity and one iteration solves the system exactly.

## ↑ Ancestors (7)

1. [Conjugate gradient method](conjugate-gradient-method.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/a/3/f/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/3/b/iv/solution.md)
