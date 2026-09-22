<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) gives the clipped boundary bounds

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\},\qquad\inf_\Omega u\geq\min\{0,\inf_{\partial\Omega}u\}.}
$$

If $c=0$, constants solve the equation, and applying these bounds after subtracting the boundary maximum or minimum gives the sharper conclusion that both extrema occur on the boundary. For $c<0$, the clipping by zero is necessary in the general statement.

To prove the upper bound, write $B=\|b_1\|_\infty$ and $C_0=\|c\|_\infty$, and choose $\alpha>0$ large enough that $\lambda\alpha^2-B\alpha-C_0>0$. For $\phi(x)=e^{\alpha x_1}$, [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) gives

$$
L\phi=\phi(a_{11}\alpha^2+b_1\alpha+c)\geq\phi(\lambda\alpha^2-B\alpha-C_0)>0.
$$

Put $u_\varepsilon=u+\varepsilon\phi$. Then $Lu_\varepsilon>0$. If $u_\varepsilon$ had a positive maximum at an interior point, its [gradient](../../../../../../gradient.md) would vanish there and its [Hessian matrix](../../../../../../hessian-matrix.md) would be [negative semidefinite](../../../../../../negative-semidefinite-matrix.md). Only the symmetric part of $a_{ij}$ contracts with this [Hessian](../../../../../../hessian-matrix.md), and its positive definiteness implies $a_{ij}D_{ij}u_\varepsilon\leq0$. Also $cu_\varepsilon\leq0$. These facts would give $Lu_\varepsilon\leq0$, a contradiction.

Since $\overline\Omega$ is compact and $u_\varepsilon$ is continuous on it, its maximum exists. It is therefore either nonpositive or attained on the boundary, proving $\sup_\Omega u_\varepsilon\leq\max\{0,\sup_{\partial\Omega}u_\varepsilon\}$. The exponential is bounded on the bounded domain; letting $\varepsilon\downarrow0$ proves the upper estimate. Apply the same argument to $-u$ for the lower estimate. This is the [exponential perturbation proof of the weak maximum principle with drift](../../../../../../exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift.md) and requires no continuity of the coefficient functions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
