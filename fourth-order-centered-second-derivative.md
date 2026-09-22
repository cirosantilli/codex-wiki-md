# Fourth-order centered second derivative

↑ **Parent:** [Central finite difference](central-finite-difference.md)

This symmetric [finite difference method](finite-difference-method.md) approximates a second derivative with $D_{4,h}u=u''-h^4u^{(6)}/90+O(h^6)$ for sufficiently [smooth](smooth-function.md) functions. Matching the constant, second-derivative and fourth-derivative coefficients of a symmetric five-node [Taylor expansion](taylor-expansion.md) determines the displayed weights uniquely; its sixth-derivative coefficient is nonzero. The [Fourier symbol](fourier-symbol-of-a-difference-operator.md) is $-4h^{-2}\sin^2(\theta/2)[1+\sin^2(\theta/2)/3]\le0$. Thus the semidiscrete [heat equation](heat-equation.md) $\dot U=D_{4,h}U$ is contractive in the discrete [L2 norm](l2-norm.md) by the [discrete Parseval identity](discrete-parseval-identity.md). This says nothing by itself about stability of a subsequently chosen time update.

## ↑ Ancestors (8)

1. [Central finite difference](central-finite-difference.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/3/b/solution.md)
