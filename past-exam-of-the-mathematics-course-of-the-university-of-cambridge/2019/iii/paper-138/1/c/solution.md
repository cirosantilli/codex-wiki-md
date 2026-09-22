<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [radical of a module](../../../../../../radical-of-a-module.md) is the smallest submodule $N\subseteq M$ for which $M/N$ is a [semisimple module](../../../../../../semisimple-module.md). Consequently, if

$$
M=M_0\supseteq M_1\supseteq M_2\supseteq\cdots
$$

has semisimple successive quotients, then $J(M_i)\subseteq M_{i+1}$. Induction gives

$$
J^i(M)\subseteq M_i,
$$

so the [radical series of a module](../../../../../../radical-series-of-a-module.md) descends at least as fast as every such series.

Dually, the [socle](../../../../../../socle-mathematics.md) is the largest semisimple submodule. If

$$
0=N_0\subseteq N_1\subseteq N_2\subseteq\cdots
$$

has semisimple successive quotients, induction in $M/N_i$ gives

$$
N_i\subseteq\operatorname{Soc}^i(M),
$$

so the [socle series of a module](../../../../../../socle-series-of-a-module.md) ascends at least as fast as every such series.

Both series terminate because $M$ has finite [composition length](../../../../../../composition-length.md). More precisely,

$$
J^i(M)=J(A)^iM,
\qquad
\operatorname{Soc}^i(M)=\{x\in M:J(A)^ix=0\}.
$$

Thus $J^r(M)=0$ exactly when $J(A)^r$ annihilates all of $M$, which is exactly when $\operatorname{Soc}^r(M)=M$. The two least terminating indices therefore coincide:

$$
\boxed{m=n=\text{the Loewy length of }M.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
