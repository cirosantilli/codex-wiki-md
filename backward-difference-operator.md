# Backward difference operator

↑ **Parent:** [Finite difference method](finite-difference-method.md)

The scaled backward [finite difference](finite-difference-split.md) uses the current and preceding nodal values to approximate a first [derivative](derivative.md). If a [function](function-split.md) has two continuous [derivatives](derivative.md), [Taylor's theorem](taylor-s-theorem.md) gives $D_h^-u(x)=u'(x)-hu''(x)/2+o(h)$ as $h\to0$. Composition with the scaled [forward difference operator](forward-difference-operator.md) gives $D_h^+D_h^-u(x)=(u(x+h)-2u(x)+u(x-h))/h^2$, the [second-order central difference](second-order-central-difference.md) for the [second derivative](second-derivative.md).

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/1/b/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/1/d/solution.md)
