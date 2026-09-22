<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The strict [null space property](../../../../../../nullspace-property.md) of order $s$ is

$$
\boxed{\|v_S\|_1<\|v_{S^c}\|_1\quad\text{for every }0\ne v\in\ker A\text{ and every }|S|\le s.}
$$

Here $v_S$ agrees with $v$ on $S$ and is zero elsewhere. Suppose a nonzero null [vector](../../../../../../vector.md) had at most $2s$ nonzero entries. Split its [support of a vector](../../../../../../support-of-a-vector.md) into disjoint sets $S,T$ of size at most $s$. Applying the [null space property](../../../../../../nullspace-property.md) to both sets would give $\|v_S\|_1<\|v_T\|_1$ and $\|v_T\|_1<\|v_S\|_1$, a contradiction. Empty parts cause the same contradiction. Thus no such nonzero null [vector](../../../../../../vector.md) exists.

For an $s$-sparse $x$, the feasible [vector](../../../../../../vector.md) $x$ has $\|x\|_0\le s$, where the zero-subscript quantity counts nonzero entries and is not a [norm](../../../../../../norm.md). Any feasible competitor $z$ with $\|z\|_0\le\|x\|_0$ also has at most $s$ nonzero entries. The difference $z-x\in\ker A$ has at most $2s$ nonzero entries, so $z=x$. Competitors with larger support have strictly larger objective. Therefore **every s-sparse [vector](../../../../../../vector.md) is the unique sparsest feasible [vector](../../../../../../vector.md)**. This is [sparse injectivity](../../../../../../sparse-injectivity.md); for $s=0$ the only sparse [vector](../../../../../../vector.md) is zero and the conclusion is immediate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
