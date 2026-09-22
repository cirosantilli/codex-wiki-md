# Transportation dual potentials

↑ **Parent:** [Transportation problem](transportation-problem.md)

Row and column potentials satisfying the displayed inequalities give a lower bound on the cost of every feasible shipment matrix: $\sum_{ij}c_{ij}x_{ij}\geq\sum_i u_i s_i+\sum_jv_j d_j$, since row sums are supplies $s_i$ and column sums are demands $d_j$. The [reduced costs](reduced-cost.md) are $c_{ij}-u_i-v_j$. A feasible matrix using only zero-reduced-cost cells attains the lower bound, proving optimality by [weak duality](weak-duality.md). The [transportation simplex algorithm](transportation-simplex-algorithm.md) sets these potentials by equality on a [transportation spanning tree](transportation-spanning-tree.md), and enters a negative-reduced-cost cell if one exists.

**Table of contents**

- [Transportation dual certificate with capacity inequalities](transportation-dual-certificate-with-capacity-inequalities.md)

## ↑ Ancestors (7)

1. [Transportation problem](transportation-problem.md)
2. [Linear programming duality](linear-programming-duality.md)
3. [Linear programming](linear-programming.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/14d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/15h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/c/solution.md)
