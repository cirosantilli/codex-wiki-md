<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Condition on the information through time $n-1$. Independence of $ξ_n$ and the definition of the [Bellman equation for terminal-wealth utility](../../../../../../bellman-equation-for-terminal-wealth-utility.md) imply

$$
\mathbb E[V(n,X_n)\mid\mathcal F_{n-1}]\leq V(n-1,X_{n-1}),
$$

because the actual holding is one candidate in the supremum. Thus $V(n,X_n)$ is a [supermartingale](../../../../../../supermartingale.md) for every strategy.

For the stated strategy it is a [martingale](../../../../../../martingale-split.md), so

$$
\mathbb E[U(X_N^*)]=V(0,X_0).
$$

Every competing strategy has expected terminal value at most $V(0,X_0)$ by the supermartingale inequality from part (a), evaluated at the bounded time $N$. Hence $θ^*$ is optimal.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
