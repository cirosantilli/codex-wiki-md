<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an effective enumeration $\varphi_0,\varphi_1,\ldots$ of unary partial computable functions. The [diagonal halting set](../../../../../../diagonal-halting-set.md) is

$$
K=\{e:\varphi_e(e)\downarrow\}.
$$

It is a [computably enumerable set](../../../../../../recursively-enumerable-set.md): on input $e$, simulate $\varphi_e(e)$ and accept if that computation halts.

Suppose $K$ were a [computable set](../../../../../../computable-set.md). A program could then halt on input $e$ exactly when the decider says $e\notin K$. Let $d$ be its own index. If $d\in K$, the program does not halt, while if $d\notin K$, it halts. Both alternatives contradict the definition of $K$. **Thus $K$ is computably enumerable but not computable.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
