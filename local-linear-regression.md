# Local linear regression

↑ **Parent:** [Local polynomial regression](local-polynomial-regression.md)

Local linear regression fits $a+b(X_i-x)$ to responses near each target $x$ by [weighted least squares](weighted-least-squares.md), then returns the fitted intercept. With weights $w_i=K((X_i-x)/h)$, put $S_k=\sum_iw_i(X_i-x)^k$ and $T_k=\sum_iw_i(X_i-x)^kY_i$. If $S_0S_2-S_1^2>0$, then $\widehat f(x)=(S_2T_0-S_1T_1)/(S_0S_2-S_1^2)$. Its [polynomial reproduction property of local polynomial regression](polynomial-reproduction-property-of-local-polynomial-regression.md) reproduces affine functions, reducing boundary bias relative to a local constant fit.

## ↑ Ancestors (8)

1. [Local polynomial regression](local-polynomial-regression.md)
2. [Nonparametric regression](nonparametric-regression.md)
3. [Nonparametric statistics](nonparametric-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/5/c/solution.md)
