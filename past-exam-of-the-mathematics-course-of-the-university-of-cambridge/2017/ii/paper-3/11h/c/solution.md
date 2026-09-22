<h1 id="11h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use uniform finite-stage enumerations $W_{n,s}$ and $K_s$. Define a uniformly [recursively enumerable](../../../../../../recursively-enumerable-set.md) [set](../../../../../../set-split.md)

$$
 V_n=\{x:\exists s\ (x\in K_s\text{ and }x<|W_{n,s}|)\}.
$$

The [S-m-n theorem](../../../../../../smn-theorem.md) supplies a total computable index function $f$ with $W_{f(n)}=V_n$. If $W_n$ is finite of size $h$, then $V_n\subseteq\{0,\ldots,h-1\}$, so $V_n$ is [recursive](../../../../../../computable-set.md). If $W_n$ is infinite, then for every $x\in K$ a sufficiently late stage has both $x\in K_s$ and $|W_{n,s}|>x$, while no $x\notin K$ is ever enumerated. Hence $V_n=K$, which is not [recursive](../../../../../../computable-set.md). Therefore $\boxed{n\in P\iff f(n)\in Q,\quad P\leq_mQ}$. As usual the effective numbering indexes all programs; if malformed codes are included, send them to a fixed index of $K$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
