# Euler one-step defect

↑ **Parent:** [Euler method](euler-method.md)

For a smooth solution of $y'=f(x,y)$, [Taylor's theorem](taylor-s-theorem.md) gives the displayed [local truncation error](local-truncation-error.md) when an [Euler method](euler-method.md) step starts at an exact solution value. Thus the one-step defect is $O(h^2)$. Dividing it by $h$ gives a [normalized local truncation error](normalized-local-truncation-error.md) of $O(h)$; these are different conventions for reporting the same residual. Also $y''=f_x+f_yf$ along the solution by the [chain rule](chain-rule.md). A global $O(h)$ error conclusion additionally requires the usual regularity and stability control over successive steps.

## ↑ Ancestors (7)

1. [Euler method](euler-method.md)
2. [Linear stability domain](linear-stability-domain.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/discrete-mathematics-continuous-mathematics-and-probability/6/c/ii/solution.md)
