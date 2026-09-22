<h1 id="2b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The constant solutions are [fixed points](../../../../../../fixed-point.md) of $G(u)=u^2(1+u)/2$. Solving $G(u)=u$ gives $u(u+2)(u-1)=0$, hence $u_*=0,-2,1$. For a [discrete dynamical system](../../../../../../discrete-dynamical-system.md), a small perturbation satisfies $\eta_{n+1}=G'(u_*)\eta_n+O(\eta_n^2)$, where

$$
G'(u)=u+\frac32u^2,\qquad G'(0)=0,\quad G'(-2)=4,\quad G'(1)=\frac52.
$$

A multiplier of magnitude less than one contracts perturbations; a multiplier greater than one expands them. Therefore **$u=0$ is asymptotically stable, while $u=-2$ and $u=1$ are unstable**. In particular, if $|u|\leq1/2$, then $|G(u)|\leq(3/4)|u|^2\leq(3/8)|u|$, proving convergence to zero without relying solely on the vanishing linear multiplier.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2B](../../2b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
