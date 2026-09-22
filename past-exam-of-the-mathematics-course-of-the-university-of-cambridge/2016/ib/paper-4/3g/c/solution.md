<h1 id="3g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $F_i(x)=a_i+\frac16\sum_{j\ne i}\sin x_j$. Solving the system is equivalent to finding a [fixed point](../../../../../../fixed-point.md) of $F:\mathbb R^3\to\mathbb R^3$. The [mean value theorem](../../../../../../mean-value-theorem.md) implies $|\sin u-\sin v|\leq|u-v|$. In the specified metric,

$$
\begin{aligned}
d(F(x),F(y))&\leq\frac16\sum_{i=1}^3\sum_{j\ne i}|x_j-y_j|\\
&=\frac13\sum_{j=1}^3|x_j-y_j|=\frac13d(x,y).
\end{aligned}
$$

Each coordinate difference occurs exactly twice. This metric makes $\mathbb R^3$ a nonempty [complete metric space](../../../../../../complete-metric-space.md), because a [Cauchy sequence](../../../../../../cauchy-sequence.md) in it is Cauchy in each real coordinate, and coordinate convergence implies convergence in the sum metric. Thus $F$ is a [contraction mapping](../../../../../../contraction-mapping.md) with constant $1/3$.

**There is exactly one solution for every choice of $(a_1,a_2,a_3)$**, by the [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md). Iteration of $F$ from any starting vector also constructs it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3G](../../3g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
