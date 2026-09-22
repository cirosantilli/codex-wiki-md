# Optimal fixed step for quadratic gradient descent

↑ **Parent:** [Fixed-step gradient descent on a positive-definite quadratic](fixed-step-gradient-descent-on-a-positive-definite-quadratic.md)

For a fixed [symmetric matrix](symmetric-matrix.md) and [positive-definite matrix](positive-definite-matrix.md) $A$, what positive [step size](step-size.md) minimizes the largest coordinate error multiplier over all [eigenvector](eigenvector.md) directions? Let $m=\lambda_{\min}>0$ and $L=\lambda_{\max}$. Since $|1-\eta\lambda|$ is a [convex function](convex-function.md) of $\lambda$, its maximum over the [eigenvalues](eigenvalue.md) occurs at an endpoint:

$$
\rho(\eta)=\max\{|1-\eta m|,|1-\eta L|\}.
$$

Balance the two extremes by solving $1-\eta m=-(1-\eta L)$:

$$
\eta_* = \frac2{m+L},\qquad \rho_* = \frac{L-m}{L+m}=\frac{\kappa-1}{\kappa+1},\qquad \kappa=\frac Lm.
$$

Here $\kappa$ is the [Euclidean norm](euclidean-norm.md) [condition number](condition-number.md) of $A$. This balance is optimal: for $\eta<\eta_*$ the endpoint $1-\eta m$ exceeds $\rho_*$, and for $\eta>\eta_*$ the endpoint $\eta L-1$ exceeds $\rho_*$. The optimal worst-case energy factor is $\rho_*^2$, rather than $\rho_*$. This optimizes a uniform one-step bound; a particular initial error supported on fewer [eigenvectors](eigenvector.md) can have a different best [step size](step-size.md).

In the example $m=1$, $L=9$, so $\eta_*=0.2$ and $\rho_*^2=0.64$. Both [eigenvalue](eigenvalue.md) directions attain that energy factor, making the displayed history exact. The smaller [step size](step-size.md) $0.1$ instead gives

$$
E_k=2(0.81)^k+\frac92(0.01)^k.
$$

Its first step reaches $E_1=1.665$, below $4.16$ for $\eta=0.2$, but subsequent progress is limited by the first direction's energy factor $0.81$. By $k=5$, the energies are approximately $0.69736$ and $0.69793$, respectively; by $k=6$, the $0.2$ iteration is ahead. A better first step need not yield a faster long-run history.

As the [condition number](condition-number.md) grows, $\rho_*$ approaches one: stability in the direction of the largest [eigenvalue](eigenvalue.md) forces small movement along the smallest-[eigenvalue](eigenvalue.md) direction. This is a precise reason to improve scaling or use a method such as the [Conjugate gradient method](conjugate-gradient-method.md), rather than merely increasing the [step size](step-size.md). When $m=L$, choosing $\eta=1/m$ eliminates every error component in one step.

## ↑ Ancestors (7)

1. [Fixed-step gradient descent on a positive-definite quadratic](fixed-step-gradient-descent-on-a-positive-definite-quadratic.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
