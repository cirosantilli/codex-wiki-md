<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

[Completing the square](../../../../../completing-the-square.md) gives

$$
c(x,a)=(a+Q^{-1}Sx)^TQ(a+Q^{-1}Sx)+x^T(R-S^TQ^{-1}S)x.
$$

Since $Q$ is [positive-definite](../../../../../positive-definite-bilinear-form.md), the unique minimizer is $\boxed{a=-Q^{-1}Sx}$ and the minimum is $\boxed{x^T(R-S^TQ^{-1}S)x}$.

The [Bellman equation](../../../../../bellman-equation.md) is $V(n,x)=x^T\Pi_0x$ and

$$
V(k,x)=\inf_a\{c(x,a)+\mathbb E[V(k+1,Ax+Ba+\epsilon_{k+1})]\}.
$$

Suppose $V(k+1,z)=z^T\Pi_rz+\gamma_{k+1}$, where $r=n-k-1$. Zero noise mean gives the expected quadratic $(Ax+Ba)^T\Pi_r(Ax+Ba)+\operatorname{tr}(\Pi_rN_{k+1})$. Complete the square again, with $Q_r=Q+B^T\Pi_rB$ and $S_r=S+B^T\Pi_rA$. This yields the [discrete Riccati recurrence](../../../../../discrete-riccati-recurrence.md)

$$
\boxed{\Pi_{r+1}=R+A^T\Pi_rA-S_r^TQ_r^{-1}S_r,\qquad K_r=-Q_r^{-1}S_r.}
$$

The matrices $Q_r$ are positive definite. The minimum of the nonnegative stage-plus-future quadratic is nonnegative, so each $\Pi_r$ is symmetric [positive semidefinite](../../../../../positive-semidefinite-matrix.md). Starting from $\gamma_n=0$, the constants obey

$$
\boxed{\gamma_k=\gamma_{k+1}+\operatorname{tr}(\Pi_{n-k-1}N_{k+1})=\sum_{j=k}^{n-1}\operatorname{tr}(\Pi_{n-j-1}N_{j+1}).}
$$

Induction proves $V(k,x)=x^T\Pi_{n-k}x+\gamma_k$, with optimal [feedback control](../../../../../closed-loop-control.md) $U_k=K_{n-k-1}X_k$.

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
