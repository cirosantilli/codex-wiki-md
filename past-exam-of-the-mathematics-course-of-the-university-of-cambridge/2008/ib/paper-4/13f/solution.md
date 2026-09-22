<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Two [norms](../../../../../norm.md) $\|\cdot\|_a,\|\cdot\|_b$ are [Lipschitz equivalent norms](../../../../../equivalent-norms.md) when constants $c,C>0$ satisfy $c\|x\|_a\leq\|x\|_b\leq C\|x\|_a$ for every vector $x$. Applying these inequalities to $x_j-x_k$ shows that a sequence is a [Cauchy sequence](../../../../../cauchy-sequence.md) for one [norm](../../../../../norm.md) exactly when it is so for the other; applying them to $x_j-x$ likewise equates convergence. If one [norm](../../../../../norm.md) is complete, a [Cauchy sequence](../../../../../cauchy-sequence.md) for the other converges using the first [norm](../../../../../norm.md) and hence also the second. Interchanging the [norms](../../../../../norm.md) proves **completeness is preserved in both directions**.

Write $x=\sum_i x_ie_i$ and set $C=\sum_i\|e_i\|$. If $\|x\|_2=1$, then $|x_i|\leq1$, and the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|x\|\leq\sum_i|x_i|\|e_i\|\leq C.
$$

Scaling a nonzero $x$ gives $\|x\|\leq C\|x\|_2$ for every $x$. The reverse [triangle inequality](../../../../../triangle-inequality.md) now implies

$$
\bigl|\|x\|-\|y\|\bigr|\leq\|x-y\|\leq C\|x-y\|_2,
$$

so $x\mapsto\|x\|$ is continuous, indeed Lipschitz, in the [Euclidean norm](../../../../../euclidean-norm.md).

Suppose there were no positive lower bound on the Euclidean [unit sphere](../../../../../unit-sphere.md). We could choose $x_j$ with $\|x_j\|_2=1$ but $\|x_j\|<1/j$. The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) supplies a subsequence converging in the [Euclidean norm](../../../../../euclidean-norm.md) to $x$. Continuity of both [norms](../../../../../norm.md) gives $\|x\|_2=1$ and $\|x\|=0$, contradicting definiteness. Therefore some $m>0$ satisfies $\|x\|\geq m$ on the unit sphere. Scaling again proves the [finite-dimensional equivalence of norms](../../../../../finite-dimensional-equivalence-of-norms.md):

$$
\boxed{m\|x\|_2\leq\|x\|\leq\left(\sum_{i=1}^n\|e_i\|\right)\|x\|_2\quad\text{for every }x\in\mathbb R^n.}
$$

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
