<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Let $[A\mid b]$ be the [augmented matrix](../../../../../augmented-matrix.md) of the [linear system](../../../../../system-of-linear-equations.md). Consistency means that $b$ is in the [column space](../../../../../column-space.md) of $A$, equivalently $\operatorname{rank}[A\mid b]=\operatorname{rank}A$. For a consistent system, choosing one solution $x_0$ gives every solution as $x_0+\ker A$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) therefore gives the complete classification:

- **Unique:** $\operatorname{rank}A=3$, equivalently $\det A\ne0$.
- **Infinitely many:** $\operatorname{rank}[A\mid b]=\operatorname{rank}A<3$.
- **None:** $\operatorname{rank}[A\mid b]>\operatorname{rank}A$.

For the given equations, subtracting the first from the second and the second from the third gives

$$
(\lambda-1)z=1,\qquad y=2.
$$

If $\lambda=0$, then $z=-1$ and the first equation gives $x=0$. If $\lambda=1$, the first reduced equation is $0=1$, so the system is inconsistent. Thus

$$
\boxed{\lambda=0:\ (x,y,z)=(0,2,-1);\qquad
\lambda=1:\ \text{no solution}.}
$$

These conclusions can also be checked from $\det A=1-\lambda$, but the row differences exhibit the inconsistency directly.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
