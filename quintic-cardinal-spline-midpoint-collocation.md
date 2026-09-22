# Quintic cardinal spline midpoint collocation

↑ **Parent:** [Cardinal B-spline](cardinal-b-spline.md)

Sampling consecutive order-six [Cardinal B-splines](cardinal-b-spline.md) at their support midpoints gives the displayed finite [B-spline collocation matrix](b-spline-collocation-matrix.md). No exterior columns are retained. Its row [strict diagonal dominance](strictly-diagonally-dominant-matrix.md) margin is at least $(66-2\cdot26-2)/120=1/10$, so the [inverse infinity-norm bound from diagonal dominance](inverse-infinity-norm-bound-from-diagonal-dominance.md) gives $\|A^{-1}\|_{\ell^\infty}\le10$. The uniform knot samples are $N_{0,6}(0),\ldots,N_{0,6}(6)=(0,1,26,66,26,1,0)/120$, obtained recursively from the [Cox-de Boor recurrence](cox-de-boor-recursion-formula.md).

## ↑ Ancestors (9)

1. [Cardinal B-spline](cardinal-b-spline.md)
2. [B-spline](b-spline.md)
3. [Spline approximation](spline-approximation.md)
4. [Spline (mathematics)](spline-mathematics.md)
5. [Uniform approximation](uniform-approximation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-61/4/c/solution.md)
