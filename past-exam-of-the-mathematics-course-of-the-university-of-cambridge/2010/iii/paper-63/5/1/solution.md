<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $h=\Delta x=1/N$ and collect only the interior values, so the actual vector dimension is $(N-1)^2$. The PDF's $N^2$ [matrix](../../../../../../matrix.md) size and its indices $k,l$ are inconsistent with the declared interior grid $m,k=1,\ldots,N-1$; neither affects the following stability argument when the interior indexing is used consistently.

Use the discrete [L2 norm](../../../../../../l2-norm.md) $\|u\|_h^2=h^2\sum_{m,k=1}^{N-1}|u_{m,k}|^2$, extending $u$ by zero to the boundary. Let $A$ be the horizontal flux operator and $B$ the vertical one. Each face coefficient is shared by its two adjacent grid values, so [summation by parts](../../../../../../abel-s-summation-formula.md) gives

$$
\langle u,Au\rangle_h=-\sum_{k=1}^{N-1}\sum_{m=0}^{N-1}
a_{m+1/2,k}|u_{m+1,k}-u_{m,k}|^2,
$$



$$
\langle u,Bu\rangle_h=-\sum_{m=1}^{N-1}\sum_{k=0}^{N-1}
a_{m,k+1/2}|u_{m,k+1}-u_{m,k}|^2.
$$

All boundary-face terms are included. Positivity of $a$ makes $A,B$ symmetric negative definite on the interior grid: zero in either energy sum forces each corresponding grid line to be constant, and its zero boundary endpoint forces that constant to vanish. Consequently

$$
\frac d{dt}\|u(t)\|_h^2=2\operatorname{Re}\langle u,(A+B)u\rangle_h\le0,
\qquad
\boxed{\|u(t)\|_h\le\|u(0)\|_h.}
$$

This bound is independent of the spatial mesh, proving semidiscrete stability. No time integrator or time-step restriction has yet been introduced.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [5](../../5.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
