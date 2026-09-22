# Steepest-descent step size

↑ **Parent:** [Exact line search for a positive-definite quadratic](exact-line-search-for-a-positive-definite-quadratic.md)

For a real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $A$ and nonzero [linear-system residual](linear-system-residual.md) $r=b-Ax$, minimize $f(x+\alpha r)$ for $f(x)=x^TAx/2-b^Tx$. Differentiating with respect to $\alpha$ gives $-r^Tr+\alpha r^TAr=0$, yielding the displayed positive step. Positive definiteness makes it the unique minimum along the line. Applying the same quotient to a nonsymmetric or indefinite matrix is a formal iteration, but this minimization proof and its convergence consequences no longer apply.

## ↑ Ancestors (7)

1. [Exact line search for a positive-definite quadratic](exact-line-search-for-a-positive-definite-quadratic.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/digital-systems-linear-algebra-introduction-to-formal-proof/6/c/i/solution.md)
