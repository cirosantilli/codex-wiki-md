<h1 id="30l/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $M\succeq0$ but $M\notin S$, its eigenvalues satisfy

$$
\sum_{i=1}^d\mu_i=\operatorname{Tr}M>s.
$$

The continuous decreasing function

$$
q(\rho)=\sum_{i=1}^d(\mu_i-\rho)_+
$$

falls from $q(0)>s$ to zero, so there is a unique $\rho>0$ for which $q(\rho)=s$.

Put

$$
p_i=(\mu_i-\rho)_+,
\qquad
\Pi=\sum_{i=1}^dp_iv_iv_i^T.
$$

Then $\Pi\succeq0$ and $\operatorname{Tr}\Pi=\sum_i p_i=s$, so $\Pi\in S$. Moreover

$$
A:=M-\Pi
=\sum_i\min(\mu_i,\rho)v_iv_i^T,
$$

and therefore

$$
0\preceq A\preceq\rho I.
$$

For any $Z\in S$,

$$
\operatorname{Tr}(AZ)\leq\rho\operatorname{Tr}Z\leq\rho s.
$$

Whenever $p_i>0$, the corresponding eigenvalue of $A$ is exactly $\rho$, while terms with $p_i=0$ contribute nothing. Consequently

$$
\operatorname{Tr}(A\Pi)=\rho\sum_i p_i=\rho s.
$$

It follows that

$$
\langle M-\Pi,Z-\Pi\rangle_F
=\operatorname{Tr}(AZ)-\operatorname{Tr}(A\Pi)\leq0.
$$

Part (a), equivalently the formula for [projection onto a positive semidefinite trace ball](../../../../../../projection-onto-a-positive-semidefinite-trace-ball.md), now gives

$$
\boxed{\pi(M)=\sum_{i=1}^d
\max(0,\mu_i-\rho)v_iv_i^T},
\qquad
\sum_i\max(0,\mu_i-\rho)=s.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30L](../../30l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
