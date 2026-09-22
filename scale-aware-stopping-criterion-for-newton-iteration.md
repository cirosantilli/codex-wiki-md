# Scale-aware stopping criterion for Newton iteration

↑ **Parent:** [Machine epsilon](machine-epsilon.md)

Near a well-conditioned simple root, a numerically stable [Newton root-finding iteration](newton-root-finding-iteration.md) cannot usually resolve steps far below the local spacing of [floating-point numbers](floating-point-number.md). That spacing has relative scale comparable to [machine epsilon](machine-epsilon.md) $\epsilon$, motivating the displayed position-based criterion with a modest constant $C$. It combines an absolute scale near zero with a relative scale for large inputs. A residual-only test is changed by rescaling the equation, whereas the root and exact Newton step are unchanged. A tiny step alone is not a universal accuracy certificate: derivative errors, stagnation and cycles require separate consideration.

## ↑ Ancestors (7)

1. [Machine epsilon](machine-epsilon.md)
2. [Floating-point arithmetic](floating-point-arithmetic-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/6/f/solution.md)
