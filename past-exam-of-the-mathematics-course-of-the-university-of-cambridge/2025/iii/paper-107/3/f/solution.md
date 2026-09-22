<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Leray-Schauder fixed point theorem](../../../../../../leray-schauder-fixed-point-theorem.md) says that a continuous compact map $T$ on a [Banach space](../../../../../../banach-space-split.md) has a fixed point if the homotopy set

$$
\{u:u=tT(u)\text{ for some }0\leq t\leq1\}
$$

is bounded. If $u=tT(u)$ with $t>0$, multiplying the equation for $T(u)$ by $t$ shows that $u$ solves

$$
\bar a^{ij}(x,u,Du)D_{ij}u+t\bar b(x,u,Du)=0
\quad\text{in }\Omega,
\qquad u=t\varphi\quad\text{on }\partial\Omega.
$$

The case $t=0$ gives $u=0$. Therefore it is enough to prove one uniform $C^{1,\beta}$ estimate for all solutions of this family and all $t\in[0,1]$. The theorem then yields a fixed point $u=T(u)$, which solves the original quasilinear problem.

Initially the construction gives $u\in C^{2,\alpha\beta}$. This makes $u$ and $Du$ Lipschitz, so composing the original $C^{0,\alpha}$ coefficients with the jet of $u$ produces $C^{0,\alpha}$ coefficients. A second application of the [global Schauder estimate](../../../../../../global-schauder-estimate.md) gives $u\in C^{2,\alpha}(\overline\Omega)$. The fixed-point theorem is an existence result and supplies no uniqueness.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
