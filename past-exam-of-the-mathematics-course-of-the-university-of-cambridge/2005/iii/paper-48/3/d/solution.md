<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Refining time alone converges to the fixed-grid, spatially discretized solution**, assuming the time-dependent coefficients and boundary forcing are suitably regular. In time-to-maturity $\tau=T-t$, the grid values solve a finite system $dU/d\tau=A_h(\tau)U+F_h(\tau)$. For fixed $h$, the [explicit Euler method](../../../../../../euler-method.md) converges to this system as $k\downarrow0$; time-step error decreases to zero.

The spatial [finite difference](../../../../../../finite-difference-split.md) error remains. Thus the limit is not in general the exact continuous pricing solution: sufficiently small time steps reveal an error plateau of order $h^2$ under the usual smooth-solution assumptions. A truncated-domain boundary error also remains fixed unless negligible as stipulated.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
