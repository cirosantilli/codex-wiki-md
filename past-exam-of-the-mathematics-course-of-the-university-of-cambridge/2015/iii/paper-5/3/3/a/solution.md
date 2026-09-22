<h1 id="3/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real [weak solution](../../../../../../../weak-solution.md) $u\in H^1_{\mathrm{loc}}(B_1)$, $\int A\nabla u\cdot\nabla\phi=0$ for compactly supported $H^1$ tests. The symmetric coefficient bounds give $A\xi\cdot\xi\ge\lambda|\xi|^2$ and $|A\xi|\le\Lambda|\xi|$. Test with $\phi=\zeta^2u$ and apply the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md):

$$
\lambda E\le2\Lambda E^{1/2}I^{1/2},\qquad E=\int\zeta^2|\nabla u|^2,\quad I=\int u^2|\nabla\zeta|^2.
$$

Thus $E\le4R^2 I$, including $E=0$. As $\zeta=1$ on $B_{r_1}$ and has support in $B_{r_2}$,

$$
\boxed{\int_{B_{r_1}}|\nabla u|^2\le4R^2\int_{B_{r_2}}u^2|\nabla\zeta|^2.}
$$

This [Caccioppoli inequality](../../../../../../../caccioppoli-inequality.md) is valid for smooth solutions and, by density of admissible tests, for locally $H^1$ [weak solutions](../../../../../../../weak-solution.md) with bounded measurable coefficients.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
