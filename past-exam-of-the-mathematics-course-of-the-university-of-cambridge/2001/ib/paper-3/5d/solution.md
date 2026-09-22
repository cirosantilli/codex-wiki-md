<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

The equality-constrained [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) says: if $x^*$ is feasible and, for some fixed multipliers, it globally minimizes the [optimization Lagrangian](../../../../../optimization-lagrangian.md) over all $x$, then it globally minimizes the objective over feasible $x$. On the feasible set the constraint terms vanish, so the two minimizations agree. No convexity assumption is needed for this version once global minimization of the [optimization Lagrangian](../../../../../optimization-lagrangian.md) has been established.

Let $S_1=\sum_i a_i$, $S_2=\sum_i a_i^2$, and $\Delta=nS_2-S_1^2$. Since

$$
\Delta=n\sum_i(a_i-S_1/n)^2>0,
$$

the two constraints are independent. For the squared [Euclidean norm](../../../../../euclidean-norm.md) objective in the original PDF, take

$$
L(x,\lambda,\mu)=\sum_i x_i^2-2\lambda\left(\sum_i x_i-1\right)-2\mu\sum_i a_ix_i.
$$

[Completing the square](../../../../../completing-the-square.md) shows that its unique global minimizer has $x_i=\lambda+\mu a_i$. The constraints become $n\lambda+S_1\mu=1$, $S_1\lambda+S_2\mu=0$, giving $\lambda=S_2/\Delta$, $\mu=-S_1/\Delta$. The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) therefore gives

$$
\boxed{x_i^*=\frac{S_2-S_1a_i}{nS_2-S_1^2},\qquad \min\sum_i x_i^2=\frac{S_2}{nS_2-S_1^2}.}
$$

For the value, use $\sum_i(x_i^*)^2=\lambda\sum_i x_i^*+\mu\sum_i a_ix_i^*=\lambda$. Uniqueness also follows directly: for every feasible $x$, the cross term in $\sum_i(x_i-x_i^*)^2$ vanishes, so the difference of objectives equals that strictly positive sum unless $x=x^*$. This is the [minimum squared norm under two affine constraints](../../../../../minimum-squared-norm-under-two-affine-constraints.md).

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
