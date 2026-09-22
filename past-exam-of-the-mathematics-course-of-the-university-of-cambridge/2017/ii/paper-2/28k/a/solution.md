<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $x_0>0$, a positive [integer](../../../../../../integer.md) $N$, decisions based only on already observed returns, and $\mathbb E|R|<\infty$. The last is a sufficient well-posedness condition absent from the print; without moment assumptions the objectives may be infinite. Put $r=1/N$. Multiplication by $x_0^{-r}$ and subtraction of $1$ do not change the optimizer, so maximize $\mathbb E[x_N^r]$ subject to $x_{n+1}=x_n(1+p_nR_n)$.

The [Bellman equation](../../../../../../bellman-equation.md) for the [value function](../../../../../../value-function.md) is

$$
\boxed{J_N(x)=x^r,\qquad J_n(x)=\max_{0\leq p\leq1}\mathbb E[J_{n+1}(x(1+pR))].}
$$

The [expectation](../../../../../../expected-value.md) uses a fresh [independent](../../../../../../independent-random-variables.md) return, since the action is chosen before it is observed. Zero wealth remains zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
