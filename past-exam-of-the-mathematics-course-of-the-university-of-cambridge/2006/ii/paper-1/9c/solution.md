<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Let $M_{ij}=\partial y_i/\partial x_j$ be the Jacobian of an invertible change of phase coordinates, and set $K(y,t)=H(x(y),t)$. The [chain rule](../../../../../chain-rule.md) gives $\nabla_xH=M^T\nabla_yK$, whence

$$
\dot y=MJM^T\nabla_yK.
$$

Therefore the necessary and sufficient condition to retain [Hamilton's equations](../../../../../hamilton-s-equations.md) for arbitrary Hamiltonians is

$$
\boxed{MJM^T=J,}
$$

equivalently $M^TJM=J$. In one degree of freedom this is the [Poisson bracket](../../../../../poisson-bracket.md) condition $\{Q,P\}=Q_qP_p-Q_pP_q=1$.

Put $D=p^2+\alpha^2q^2$. On a smooth branch of the angular coordinate,

$$
Q_q=\frac{\alpha p}{D},\quad Q_p=-\frac{\alpha q}{D},\quad P_q=\alpha q,\quad P_p=p/\alpha.
$$

Consequently $Q_qP_p-Q_pP_q=(p^2+\alpha^2q^2)/D=1$. **The transformation is canonical for every real $\alpha\ne0$ on each angular-coordinate chart.** The origin is excluded and a single-valued arctangent cannot give a global chart on the punctured plane; using an angle modulo $2\pi$ accounts for the usual branch qualification.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
