<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose $|Dv|\leq M$. The coefficient matrices in part (ii) then have uniform ellipticity constants depending only on $M$. Applying the [Harnack inequality for uniformly elliptic divergence-form equations](../../../../../../../harnack-inequality-for-uniformly-elliptic-divergence-form-equations.md) to the nonnegative solutions $M+D_kv_R$ and $M-D_kv_R$ gives a scale-independent oscillation contraction

$$
\operatorname{osc}_{B_{1/4}}D_kv_R
\leq\theta\operatorname{osc}_{B_1}D_kv_R,
\qquad0<\theta<1.
$$

Scaling back,

$$
\operatorname{osc}_{B_{R/4}}D_kv
\leq\theta\operatorname{osc}_{B_R}D_kv.
$$

For fixed $r$, iterate this estimate with $R=4^mr$ and use the global bound $|D_kv|\leq M$ to obtain $\operatorname{osc}_{B_r}D_kv\leq2M\theta^m\to0$. Every partial derivative is therefore constant, so $v(x)=a\mathbin\cdot x+b$ is an [affine function](../../../../../../../affine-function.md). This is a bounded-gradient Bernstein theorem for entire minimal graphs.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
