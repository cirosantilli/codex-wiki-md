<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $K_{ij}=K(\mathbf x_i,\mathbf x_j)$ and $\mathbf P=\sum_i\mathbf v_i$. The unit particle [masses](../../../../mass.md) make this sum the total [momentum](../../../../momentum-split.md). Exchange the two indices and use the [symmetry](../../../../symmetry-physics.md) $K_{ij}=K_{ji}$:

$$
\dot{\mathbf P}=\sum_{i,j}K_{ij}(\mathbf v_j-\mathbf v_i)
=\frac12\sum_{i,j}K_{ij}\bigl[(\mathbf v_j-\mathbf v_i)+(\mathbf v_i-\mathbf v_j)\bigr]=\boxed{\mathbf0}.
$$

Thus every interacting pair transfers equal and opposite [momentum](../../../../momentum-split.md), even though the [velocity alignment](../../../../velocity-alignment.md) dissipates [kinetic energy](../../../../kinetic-energy.md).

For the total [kinetic energy](../../../../kinetic-energy.md) $E_N=\tfrac12\sum_i|\mathbf v_i|^2$, apply the same exchange of indices:

$$
\begin{aligned}
\dot E_N
&=\sum_{i,j}K_{ij}\mathbf v_i\cdot(\mathbf v_j-\mathbf v_i)\\
&=\frac12\sum_{i,j}K_{ij}\bigl[\mathbf v_i\cdot(\mathbf v_j-\mathbf v_i)+\mathbf v_j\cdot(\mathbf v_i-\mathbf v_j)\bigr]\\
&=\boxed{-\frac12\sum_{i,j}K_{ij}|\mathbf v_j-\mathbf v_i|^2\leq0}.
\end{aligned}
$$

The dissipated [kinetic energy](../../../../kinetic-energy.md) is that of relative motion. Since the total [momentum](../../../../momentum-split.md) is constant, $E_N-|\mathbf P|^2/(2N)=\tfrac12\sum_i|\mathbf v_i-\mathbf P/N|^2$ also decreases. Equality holds when every pair with $K_{ij}>0$ has the same [velocity](../../../../velocity.md); the hypotheses permit disconnected interacting groups, so they alone do not guarantee eventual global [velocity alignment](../../../../velocity-alignment.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
