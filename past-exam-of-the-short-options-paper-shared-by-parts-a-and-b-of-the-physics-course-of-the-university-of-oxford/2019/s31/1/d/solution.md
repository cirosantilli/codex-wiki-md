<h1 id="s31/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a smooth exact solution such as $u(x,t)=e^{-Dq^2t}\sin(qx)$ on a domain with matching boundary conditions, and compare numerical and exact values at a fixed physical time. To measure spatial order, halve $h$ while making temporal error negligible; the [error norm](../../../../../error-norm.md) should fall by a factor of four. To measure temporal order, halve $k$ on a sufficiently fine fixed spatial grid and again expect a factor of four. Report observed order $p=\log_2(E_h/E_{h/2})$ and use several refinements to identify the asymptotic regime.

Check more than one smooth mode, boundary implementation and expected conservation or decay properties. A [manufactured solution](../../../../../manufactured-solution.md) with an added known source can test nontrivial boundaries and forcing. Repeat in maximum and root-mean-square [norms](../../../../../norm.md), stop before finite-precision or solver tolerances dominate, and separate stability failures from errors in convergence order. A single small error or a single visually smooth solution does not establish accuracy.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
