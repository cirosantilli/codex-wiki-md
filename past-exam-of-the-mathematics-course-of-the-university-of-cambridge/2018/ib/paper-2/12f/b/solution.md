<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Two norms $N_1,N_2$ are [equivalent norms](../../../../../../equivalent-norms.md) when constants $c,C>0$ satisfy

$$
cN_1(v)\leq N_2(v)\leq CN_1(v)
$$

for every $v$.

For $x,y\in\mathbb R^n$, the reverse [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
|g(x)-g(y)|
\leq\left\|\sum_{i=1}^n(x_i-y_i)e_i\right\|
\leq\sum_{i=1}^n|x_i-y_i|\,\|e_i\|
\leq C_0\|x-y\|_2
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Hence $g$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md), and therefore continuous.

On the compact Euclidean [unit sphere](../../../../../../unit-sphere.md), $g$ is positive and continuous, so the [extreme value theorem](../../../../../../extreme-value-theorem.md) gives $0<m\leq g\leq M<\infty$. Homogeneity then yields

$$
m\|x\|_2\leq g(x)\leq M\|x\|_2.
$$

Thus every norm on a [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md) is equivalent to the [Euclidean norm](../../../../../../euclidean-norm.md); comparing two such bounds proves **any two norms on $V$ are Lipschitz equivalent.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
