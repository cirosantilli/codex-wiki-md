# Natural cubic cardinal spline endpoint rows

↑ **Parent:** [Cardinal cubic B-spline](cardinal-cubic-b-spline.md)

For the centered [Cardinal cubic B-spline](cardinal-cubic-b-spline.md) $\beta$ with knot values $1/6,4/6,1/6$, write $s(x)=\sum_{j=-1}^{m+1}c_j\beta(x/h-j)$ on $[0,mh]$. [interpolation](interpolation-split.md) gives $c_{i-1}+4c_i+c_{i+1}=6u(ih)$ for $i=0,\ldots,m$. Since $\beta''(0)=-2$ and $\beta''(\pm1)=1$, the natural endpoint conditions $s''(0)=s''(mh)=0$ give the displayed extra two rows. These supply the two equations missing from [interpolation](interpolation-split.md) alone.

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
