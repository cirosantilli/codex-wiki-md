<h1 id="22i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x\in X$, define $e_x\in X^{**}$ by $e_x(\phi)=\phi(x)$. The map $J:x\mapsto e_x$ is linear, and

$$
|e_x(\phi)|\le\|\phi\|\,\|x\|
$$

shows $\|Jx\|\le\|x\|$, so $J$ is continuous. The granted equality $\|Jx\|=\|x\|$ is the [canonical embedding into the bidual](../../../../../../canonical-embedding-into-the-bidual.md).

Suppose, contrary to the claim, that exactly the same linear functionals are continuous for $\|\cdot\|$ and $\|\cdot\|'$. Their common continuous dual has two operator norms, say $\|\cdot\|_*$ and $\|\cdot\|_*'$. Both dual spaces are [Banach](../../../../../../banach-space-split.md), even if the second normed space $X$ is not complete. The identity map

$$
(X^*,\|\cdot\|_*)\longrightarrow(X^*,\|\cdot\|_*')
$$

has a closed graph: convergence in either operator norm implies pointwise convergence on $X$, so two limits must agree. The [closed graph theorem](../../../../../../closed-graph-theorem.md) makes the two dual norms equivalent.

Applying the isometric bidual formula for each primal norm then gives constants $c,C>0$ such that

$$
c\|x\|\le\|x\|'\le C\|x\|
\qquad(x\in X).
$$

This says the two norms are [equivalent norms](../../../../../../equivalent-norms.md), contrary to the hypothesis. Their continuous duals must therefore differ as sets, so a linear functional belonging to one and not the other is continuous for exactly one of the two norms.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22I](../../22i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
