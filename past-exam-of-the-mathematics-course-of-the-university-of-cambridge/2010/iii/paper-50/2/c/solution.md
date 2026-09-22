<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [steady state](../../../../../../steady-state.md) is a time-independent [density operator](../../../../../../density-matrix.md) satisfying $\mathcal L(\rho_*)=0$, equivalently a constant physical [Bloch vector](../../../../../../bloch-vector.md) $s_*$ satisfying $\boxed{As_*=-c}$. Let $K=N^2-1$. By the rank criterion for a linear system, this equation has a solution exactly when

$$
\boxed{\operatorname{rank}A=\operatorname{rank}[A\mid c]}.
$$

When it is consistent, every algebraic solution has the form $s_0+v$ with $v\in\ker A$, so the solution affine space has dimension $K-\operatorname{rank}A$ by the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md). Physical [steady states](../../../../../../steady-state.md) are its intersection with the positive [density operator](../../../../../../density-matrix.md) body. The algebraic equilibrium is unique exactly when $\operatorname{rank}A=K$, in which case $\boxed{s_*=-A^{-1}c}$.

An arbitrary affine differential equation need not have an equilibrium: $A=0$, $c\ne0$ is inconsistent. For the finite-dimensional, time-independent [Lindblad equation](../../../../../../lindblad-equation.md) under discussion, however, **a physical steady state always exists**. Indeed, the averages $\bar\rho_T=T^{-1}\int_0^T\rho(t)\,dt$ remain positive with [trace](../../../../../../matrix-trace.md) one. Compactness supplies a convergent subsequence as $T\to\infty$, and

$$
\mathcal L(\bar\rho_T)=\frac{\rho(T)-\rho(0)}{T}\longrightarrow0.
$$

The limit is a physical [steady state](../../../../../../steady-state.md), proving that [Finite-dimensional Lindbladians have stationary states](../../../../../../finite-dimensional-lindbladians-have-stationary-states.md) and that the rank consistency condition is automatically satisfied for this physical generator.

In this setting, full rank also characterizes uniqueness among physical [steady states](../../../../../../steady-state.md). To justify the converse when $A$ is singular, a nonzero $v\in\ker A$ gives a fixed traceless [Hermitian operator](../../../../../../hermitian-operator.md) $X=\sum_kv_k\sigma_k$. Write its [positive-negative decomposition](../../../../../../positive-negative-decomposition-of-a-hermitian-operator.md) $X=X_+-X_-$. Time-average the evolutions of the two positive operators along a common convergent subsequence; the limits $Y_\pm$ are positive stationary operators and satisfy $X=Y_+-Y_-$. Their traces are equal because $\operatorname{Tr}X=0$. If there were only one stationary [density operator](../../../../../../density-matrix.md), both $Y_\pm$ would be this matrix times the same [trace](../../../../../../matrix-trace.md), forcing $X=0$, a contradiction. Hence $\boxed{\text{unique physical steady state}\iff\operatorname{rank}A=N^2-1}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
