# Three-point asymmetric second-derivative formula

↑ **Parent:** [Finite difference](finite-difference-split.md)

Matching the monomials $1,x,x^2$ gives $f''(2)\approx(2/3)f(0)-f(1)+(1/3)f(3)$. With error defined as the true derivative minus this approximation, its [Peano kernel](peano-kernel.md) is $K(\theta)=2\mathbf1_{\{\theta<2\}}+(1-\theta)_+^2-(3-\theta)^2/3$ on $[0,3]$. The derivative evaluation causes a jump at two. Applying the [Peano kernel theorem](peano-kernel-theorem.md) gives $\lambda(f)=\tfrac12\int_0^3Kf^{(3)}$.

## ↑ Ancestors (6)

1. [Finite difference](finite-difference-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/19c/solution.md)
- [Sharp error constants for a Peano kernel](sharp-error-constants-for-a-peano-kernel.md)
