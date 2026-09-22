<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With the interior ordering correction in part (a), iteration of part (c) gives

$$
\|u_k\|_{C^{2,\alpha}}\leq2^{-(k-1)}\|u_1\|_{C^{2,\alpha}}+2C.
$$

The bounded [monotone sequence](../../../../../../monotone-sequence.md) has a pointwise limit $u$. By [compact embedding of Hölder spaces](../../../../../../compact-embedding-of-holder-spaces.md), a subsequence converges in $C^{2,\beta}$ for $0<\beta<\alpha$, necessarily to this same limit. All convergent subsequences have that limit, so compactness gives convergence of the full sequence in $C^{2,\beta}$. Passing to the limit in $\Delta u_k=V(u_{k-1})$ gives the equation and boundary values. The uniform [Hölder seminorm](../../../../../../holder-seminorm.md) bounds on second derivatives pass to the limit, so $u\in C^{2,\alpha}(\overline\Omega)$, and the barriers remain ordered:

$$
\boxed{Qu=0,\qquad u|_{\partial\Omega}=\psi,\qquad \varphi^-\leq u\leq\varphi^+.}
$$

This proves the intended [monotone iteration for a semilinear elliptic equation](../../../../../../monotone-iteration-for-a-semilinear-elliptic-equation.md). With only the boundary ordering printed in the PDF, the counterexample in part (a) shows the requested trapped solution need not exist.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
