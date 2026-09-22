<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $X^{(i)}=X_{1:n}\setminus X_i$, [Han's inequality for relative entropy](../../../../../../han-s-inequality-for-relative-entropy.md) states that, when $P=\bigotimes_{i=1}^nP_i$,

$$
D(Q\Vert P)\geq\frac1{n-1}\sum_{i=1}^n
D(Q_{X^{(i)}}\Vert P_{X^{(i)}}).
$$

First prove the [chain rule for relative entropy](../../../../../../chain-rule-for-relative-entropy.md). For two coordinates,

$$
\log\frac{Q(x,y)}{P(x,y)}
=\log\frac{Q_X(x)}{P_X(x)}
+\log\frac{Q_{Y\mid X}(y\mid x)}{P_{Y\mid X}(y\mid x)}.
$$

Taking expectation under $Q$ gives

$$
D(Q_{XY}\Vert P_{XY})
=D(Q_X\Vert P_X)
+\mathbb E_{Q_X}D(Q_{Y\mid X}\Vert P_{Y\mid X}),
$$

and iteration proves the chain rule for any finite product.

Write $Q_i(\cdot\mid x_{<i})$ for the successive conditional distributions. Since $P$ is a product, the chain rule gives

$$
D(Q\Vert P)=\sum_{i=1}^n
\mathbb E_QD(Q_i(\cdot\mid X_{<i})\Vert P_i).
$$

For a fixed omitted coordinate $j$, applying the chain rule in the remaining coordinate order gives

$$
D(Q_{X^{(j)}}\Vert P_{X^{(j)}})
=\sum_{i\ne j}\mathbb E_Q
D(Q_i(\cdot\mid X_{<i}\setminus X_j)\Vert P_i).
$$

The convexity of [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) implies that removing $X_j$ from the conditioning can only decrease each averaged conditional divergence. Summing over $j$, each full conditional increment occurs for exactly the $n-1$ indices $j\ne i$, and therefore

$$
\sum_{j=1}^nD(Q_{X^{(j)}}\Vert P_{X^{(j)}})
\leq(n-1)D(Q\Vert P),
$$

which is the claimed inequality. Equivalently, this is [Han's entropy inequality](../../../../../../han-s-entropy-inequality.md) after expanding each divergence: the product-reference cross-entropy terms cancel because they are modular.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
