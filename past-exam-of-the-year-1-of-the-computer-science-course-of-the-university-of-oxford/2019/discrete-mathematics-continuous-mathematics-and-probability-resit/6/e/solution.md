<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The update in [Newton's method in optimization](../../../../../newton-s-method-in-optimization.md) is $\mathbf z_{k+1}=\mathbf z_k-H_f(\mathbf z_k)^{-1}\nabla f(\mathbf z_k)$. Substituting the previous formulas gives

$$
\mathbf z_{k+1}=\mathbf z_k-(I+\mathbf z_k\mathbf z_k^T)\mathbf z_k=-\|\mathbf z_k\|^2\mathbf z_k.
$$

Thus the distance from the unique [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) obeys **$r_{k+1}=r_k^3$**, where $r_k=\|\mathbf z_k\|$. In particular,

$$
r_k=r_0^{3^k}\longrightarrow0\qquad(0\leq r_0<1).
$$

For $0<r_0<1$, the error ratio $r_{k+1}/r_k^3$ is exactly $1$, proving exact [cubic convergence](../../../../../cubic-convergence.md). If $r_0=0$, the initial point already attains the [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md). All updates are defined because the [Hessian](../../../../../hessian-matrix.md) is invertible everywhere. This is [Newton minimization of the square-root norm](../../../../../newton-minimization-of-the-square-root-norm.md); its special update also shows why the given initial condition matters: $r_0=1$ produces an alternating two-cycle, and $r_0>1$ diverges.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
