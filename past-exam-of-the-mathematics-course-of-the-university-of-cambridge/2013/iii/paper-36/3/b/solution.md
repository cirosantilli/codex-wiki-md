<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $x$ is the unique [basis pursuit](../../../../../../basis-pursuit.md) [minimizer](../../../../../../global-minimizer.md). Fix $0\ne v\in\ker A$ and set

$$
\alpha=\langle\operatorname{sgn}(x_S),v_S\rangle,\qquad\beta=\|v_{S^c}\|_1.
$$

There is $\varepsilon>0$ such that the [sign function](../../../../../../sign-function.md) of $x_j+t v_j$ equals that of $x_j$ at every $j\in S$ whenever $|t|<\varepsilon$. To choose it, take less than the minimum of $|x_j|/|v_j|$ over the nonzero $v_j$ in $S$; if that set is empty, any positive $\varepsilon$ works. On this interval the [L1 norm](../../../../../../l1-norm.md) has the exact expression

$$
\|x+t v\|_1-\|x\|_1=t\alpha+|t|\beta.
$$

For $0<t<\varepsilon$, both $x+t v$ and $x-t v$ are distinct feasible [vectors](../../../../../../vector.md). Uniqueness forces their objective differences to be strictly positive, so $\alpha+\beta>0$ and $-\alpha+\beta>0$. Therefore

$$
\boxed{|\langle\operatorname{sgn}(x_S),v_S\rangle|<\|v_{S^c}\|_1\quad(0\ne v\in\ker A).}
$$

**The [fixed-sign null space condition](../../../../../../fixed-sign-null-space-condition.md) is necessary as well as sufficient.** This argument also covers an empty [support of a vector](../../../../../../support-of-a-vector.md): then $\alpha=0$ and the nonzero [null space](../../../../../../kernel-of-a-linear-map.md) [vector](../../../../../../vector.md) has $\beta>0$. Strictness is indispensable: equality would make a sufficiently short feasible segment have the same objective as $x$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
