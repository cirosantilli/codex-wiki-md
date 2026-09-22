<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [steady state](../../../../../steady-state.md) $\mathbf c_*$ satisfies $0=A\mathbf c_*-\mathbf b$, hence

$$
A\mathbf c_*=\mathbf b.
$$

The sign is positive on the right after rearranging the supplied equation. A solution exists exactly when $\mathbf b$ lies in the [column space](../../../../../column-space.md) of $A$, which above was found to be the zero-sum [vector subspace](../../../../../vector-subspace.md). Equivalently, multiply by the [left null space](../../../../../left-null-space.md) [vector](../../../../../vector.md) $\mathbf1^T$:

$$
\boxed{\mathbf1^T\mathbf b=b_1+b_2+b_3+b_4=0.}
$$

This condition is necessary and sufficient for an algebraic [steady state](../../../../../steady-state.md), since both the [column space](../../../../../column-space.md) and that zero-sum [vector subspace](../../../../../vector-subspace.md) have [dimension](../../../../../dimension-vector-space.md) $3$. It expresses global [conservation of mass](../../../../../mass-conservation.md): in the closed [box model](../../../../../box-model.md), total tracer production must balance total tracer removal. With the paper's convention $-\mathbf b$, a positive $b_i$ is a sink and a negative $b_i$ is a source. If the sum is nonzero, $dM/dt=-\sum_i b_i$ and the inventory changes linearly in time, preventing a [steady state](../../../../../steady-state.md).

When the condition holds, all algebraic [steady states](../../../../../steady-state.md) form the [affine solution space of a linear equation](../../../../../affine-solution-space-of-a-linear-equation.md) $\mathbf c_p+\alpha\mathbf1$, for any particular solution $A\mathbf c_p=\mathbf b$. The initial inventory selects one member through $\mathbf1^T\mathbf c_* =\mathbf1^T\mathbf c(0)$. For a physically admissible solution, its four [concentrations](../../../../../concentration.md) must additionally be nonnegative; the compatibility condition alone imposes no such inequalities.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
