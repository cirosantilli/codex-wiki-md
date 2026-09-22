<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) states that every bounded $T:H\to H$ is uniquely

$$
\boxed{T=V|T|,\qquad |T|=(T^*T)^{1/2},\qquad \ker V=\ker T,}
$$

where $V$ is a [partial isometry](../../../../../../partial-isometry.md) with initial space $\overline{\operatorname{Ran}|T|}=(\ker T)^\perp$ and final space $\overline{\operatorname{Ran}T}$. Its initial and final [orthogonal projections](../../../../../../orthogonal-projection.md) are $V^*V$ and $VV^*$.

Existence of $|T|$ was proved in (a). For every $\xi$,

$$
\||T|\xi\|^2=\langle T^*T\xi,\xi\rangle=\|T\xi\|^2.
$$

Thus the map $|T|\xi\mapsto T\xi$ is well defined and isometric on $\operatorname{Ran}|T|$. It extends uniquely to an isometry between its closed range and $\overline{\operatorname{Ran}T}$. Extend it by zero on $\ker|T|=\ker T$ to obtain $V$. The equation and the [projection](../../../../../../projection-linear-algebra.md) assertions follow immediately. Any other normalized [partial isometry](../../../../../../partial-isometry.md) with the same product must agree on the dense range of $|T|$ and vanish on its [orthogonal complement](../../../../../../orthogonal-complement.md), giving uniqueness. The [kernel](../../../../../../kernel-of-a-linear-map.md) normalization is essential; without it an action on the [kernel](../../../../../../kernel-of-a-linear-map.md) could be added.

A useful consequence for a [Von Neumann algebra](../../../../../../von-neumann-algebra.md) $M$ is that the polar factors of $T\in M$ also belong to $M$. The polynomial construction in (a) puts $|T|$ in the norm-closed algebra $M$. For $\varepsilon>0$, the inverse of $|T|+\varepsilon I$ belongs to $M$ by a convergent Neumann series, and

$$
T(|T|+\varepsilon I)^{-1}\longrightarrow V\quad\text{strongly}.
$$

These operators are contractions, since $\||T|\xi\|\leq\|(|T|+\varepsilon I)\xi\|$. On [vectors](../../../../../../vector.md) $|T|\xi$ the difference from $V$ has [norm](../../../../../../norm.md) at most $\varepsilon\|\xi\|$, and on the [kernel](../../../../../../kernel-of-a-linear-map.md) it is zero. Density and the uniform bound prove the strong limit. Strong closedness of $M$ then gives $V\in M$. This justifies the use of algebra-valued polar factors in Question 7(c).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
