# Forney algorithm

↑ **Parent:** [Error evaluator polynomial](error-evaluator-polynomial.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forney_algorithm)

For distinct error locations and the syndrome convention $S_\ell=\sum_i E_iX_i^{b+\ell}$, the displayed formula recovers the error magnitudes from the [error evaluator polynomial](error-evaluator-polynomial.md) and [error locator polynomial](error-locator-polynomial.md). At $z=X_i^{-1}$, the evaluator is $E_iX_i^b\prod_{h\ne i}(1-X_h/X_i)$, whereas the locator's [formal derivative](formal-derivative.md) is $-X_i\prod_{h\ne i}(1-X_h/X_i)$. Their quotient gives the formula; the denominator is nonzero because the locations are distinct.

// Target: polynomial.bigb

## ↑ Ancestors (9)

1. [Error evaluator polynomial](error-evaluator-polynomial.md)
2. [Error locator polynomial](error-locator-polynomial.md)
3. [BCH code](bch-code.md)
4. [Cyclic code](cyclic-code.md)
5. [Coding theory](coding-theory-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Error evaluator polynomial](error-evaluator-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-87/3/solution.md)
