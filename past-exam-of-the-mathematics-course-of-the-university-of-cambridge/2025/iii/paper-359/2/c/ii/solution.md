<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Initially $u\in H^1(\Omega)$, so in three dimensions

$$
u\in L^6,\qquad \nabla u\in L^2.
$$

Both terms in

$$
\widetilde B(u,u)
=(u\mathbin\cdot\nabla)u
+\frac12(\nabla\mathbin\cdot u)u
$$

therefore belong to $L^{3/2}$. The equation becomes

$$
-\nu\Delta u=f-\widetilde B(u,u)
\quad\hbox{with right-hand side in }L^{3/2}.
$$

Periodic [elliptic regularity](../../../../../../../elliptic-regularity.md) gives

$$
u\in W^{2,3/2}.
$$

The Sobolev embedding then yields

$$
u\in W^{1,3}\cap L^6.
$$

Consequently each product in $\widetilde B(u,u)$ belongs to $L^2$, because

$$
L^6\cdot L^3\subset L^2.
$$

A second application of [elliptic regularity](../../../../../../../elliptic-regularity.md) now gives

$$
u\in H^2_{\rm per}(\Omega)=D(\widetilde A).
$$

Every term in the equation belongs to $\widetilde H$, and hence

$$
\boxed{
u\in D(\widetilde A),
\qquad
\nu\widetilde Au+\widetilde B(u,u)=f
\quad\hbox{in }\widetilde H}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
