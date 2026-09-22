# Third-order conditions for an explicit Runge-Kutta method

↑ **Parent:** [Order of a Runge-Kutta method](order-of-a-runge-kutta-method.md)

For an explicit [Runge-Kutta method](runge-kutta-method.md) with coefficients $A,b$, put $c=A\mathbf1$ and let $c^2$ mean componentwise squaring. The conditions $b^T\mathbf1=1$, $b^Tc=1/2$, $b^Tc^2=1/3$ and $b^TAc=1/6$ match the exact flow expansion through degree three: the two cubic differentials are $f^{\prime\prime}[f,f]$ and $(f^\prime)^2f$. For sufficiently smooth vector fields these give local error $O(h^4)$ and, under the usual finite-interval [Lipschitz continuity](lipschitz-continuity.md) assumptions, global error $O(h^3)$.

## ↑ Ancestors (7)

1. [Order of a Runge-Kutta method](order-of-a-runge-kutta-method.md)
2. [Runge-Kutta method](runge-kutta-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/18c/solution.md)
