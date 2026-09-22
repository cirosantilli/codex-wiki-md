<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

For $X$ in the [dual cone](../../../../../../dual-cone.md) $C$, copositivity of $Q-\lambda I$ gives $\langle X,Q-\lambda I\rangle_F\geq0$. An upper-bounding [Lagrangian](../../../../../../lagrangian.md) for the maximization is therefore

$$
L(\lambda,X)=\lambda+\langle X,Q-\lambda I\rangle_F
=\langle Q,X\rangle_F+\lambda(1-\operatorname{tr}X).
$$

Its [supremum](../../../../../../supremum.md) over unrestricted $\lambda$ is finite precisely when $\operatorname{tr}X=1$. Minimizing that upper bound gives the [conic program](../../../../../../conic-optimization.md)

$$
\boxed{\min_{X\in C}\ \langle Q,X\rangle_F
\quad\text{subject to }\operatorname{tr}X=1}.
$$

This is [completely positive optimization](../../../../../../completely-positive-optimization.md), not simply [semidefinite programming](../../../../../../semidefinite-programming.md): $C$ is the [completely positive cone](../../../../../../completely-positive-cone.md).

There is also a direct equality certificate. Every feasible $X=\sum_j u_ju_j^T$, $u_j\geq0$, has $\sum_j\|u_j\|_2^2=1$. Its objective is a weighted average of the nonnegative-sphere [Rayleigh quotients](../../../../../../rayleigh-quotient.md), hence is at least $\alpha$. For a minimizing unit [vector](../../../../../../vector.md) $x_*$ from part (g), $X_*=x_*x_*^T$ is feasible and has objective $\alpha$. Thus $\boxed{X_*=x_*x_*^T}$ attains the dual and both values agree, without relying on unverified regularity assumptions.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
