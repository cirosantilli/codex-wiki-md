# Exact line search for a positive-definite quadratic

↑ **Parent:** [Gradient descent](gradient-descent.md)

For $f(x)=x^TAx/2-b^Tx$ with $A$ positive definite and residual $r=b-Ax$, exact line search along $r$ uses

$$
t=\frac{r^Tr}{r^TAr}.
$$

The objective error contracts by

$$
1-\frac{(r^Tr)^2}{(r^TA^{-1}r)(r^TAr)}
\leq 1-\frac{\lambda_{\min}(A)}{\lambda_{\max}(A)}.
$$

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/40c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/40a/b/iii/solution.md)
