# Cubic regression spline

↑ **Parent:** [Regression spline](regression-spline.md)

A cubic regression spline represents a mean function in a finite-dimensional space of piecewise cubic functions, with continuity of the function and its first two derivatives at chosen knots. A penalized fit minimizes a residual criterion plus $\lambda\int(f'')^2$, using $\Omega_{jk}=\int B_j''B_k''$. Unlike a full [cubic smoothing spline](cubic-smoothing-spline.md) with knots at every distinct observation, its knot set can be much smaller. The `mgcv` basis `bs="cr"` uses a penalized natural cubic regression-spline basis with linear tails.

## ↑ Ancestors (8)

1. [Regression spline](regression-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/5/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/5/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/6/e/solution.md)
