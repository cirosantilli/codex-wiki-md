# Cubic cardinal spline interpolation with two left endpoint derivatives

↑ **Parent:** [Cardinal cubic B-spline](cardinal-cubic-b-spline.md)

For knot spacing $h=1/2$ on $[0,1]$, the five translates indexed $-3,-2,-1,0,1$ span the $C^2$ piecewise cubic space. With normalized knot values $1/6,2/3,1/6$, nodal interpolation gives $(c_{-3}+4c_{-2}+c_{-1})/6=u(0)$ and the two shifted equations at $h,2h$. Left-end Hermite data give $(c_{-1}-c_{-3})/(2h)=u'(0)$ and $(c_{-3}-2c_{-2}+c_{-1})/h^2=u''(0)$. These five equations uniquely determine the coefficients. Derivative data need existence or separate prescription; continuity of $u$ alone does not supply them.

## ↑ Ancestors (10)

1. [Cardinal cubic B-spline](cardinal-cubic-b-spline.md)
2. [Cardinal B-spline](cardinal-b-spline.md)
3. [B-spline](b-spline.md)
4. [Spline approximation](spline-approximation.md)
5. [Spline (mathematics)](spline-mathematics.md)
6. [Uniform approximation](uniform-approximation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
