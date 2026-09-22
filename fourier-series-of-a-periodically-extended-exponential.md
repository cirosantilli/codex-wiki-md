# Fourier series of a periodically extended exponential

↑ **Parent:** [Fourier series](fourier-series-split.md)

Let $L>0$ and real $\kappa\ne0$. Extend $e^{\kappa x}$ with period $2L$. In the [Fourier series](fourier-series-split.md) convention $a_0/2+\sum_{n\geq1}[a_n\cos(n\pi x/L)+b_n\sin(n\pi x/L)]$, put $q_n=n\pi/L$. Direct [integration](integral-split.md) gives

$$
a_0=\frac{2\sinh(\kappa L)}{\kappa L},\qquad
a_n=\frac{2\kappa(-1)^n\sinh(\kappa L)}{L(\kappa^2+q_n^2)},\qquad
b_n=-\frac{2q_n(-1)^n\sinh(\kappa L)}{L(\kappa^2+q_n^2)}.
$$

For example, the required [antiderivatives](antiderivative.md) are $e^{\kappa x}(\kappa\cos q_nx+q_n\sin q_nx)/(\kappa^2+q_n^2)$ and $e^{\kappa x}(\kappa\sin q_nx-q_n\cos q_nx)/(\kappa^2+q_n^2)$. The [Dirichlet-Jordan convergence theorem](dirichlet-jordan-convergence-theorem.md) gives the exponential value away from the jumps and their midpoint $\cosh(\kappa L)$ at odd multiples of $L$. For $\kappa=0$, the [function](function-split.md) is identically one, with $a_0=2$ and all other [Fourier coefficients](fourier-coefficient.md) zero.

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/17/b/solution.md)
