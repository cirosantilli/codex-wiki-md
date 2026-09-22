<h1 id="11h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [S-m-n theorem](../../../../../../smn-theorem.md) says that parameters can be compiled effectively into program indices: for a standard effective numbering, there is a [total computable function](../../../../../../total-computable-function.md) $s_m^n$ with $\varphi_{s_m^n(e,\mathbf a)}(\mathbf x)=\varphi_e(\mathbf a,\mathbf x)$ for partial computable functions of $m+n$ arguments.

Write $K=\{e:\varphi_e(e)\text{ halts}\}$, a [recursively enumerable](../../../../../../recursively-enumerable-set.md) [halting problem](../../../../../../halting-problem.md). If $X$ is [recursively enumerable](../../../../../../recursively-enumerable-set.md), make a program with parameter $x$ which ignores its input and runs a semidecision procedure for $x\in X$, halting when that procedure halts. By the [S-m-n theorem](../../../../../../smn-theorem.md) its index $f(x)$ is total computable and $f(x)\in K\iff x\in X$. Conversely, $X\leq_mK$ implies that $X$ is [recursively enumerable](../../../../../../recursively-enumerable-set.md) by the previous construction. Thus $\boxed{X\text{ is r.e.}\iff X\leq_mK}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11H](../../11h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
