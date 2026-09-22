<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a finite symmetric generating set $S$ for $\Gamma$, a base point $p$, and put $L=\max_{s\in S}d(p,sp)$. If the [word length](../../../../../../word-length.md) of $\gamma$ is at most $m$, the [triangle inequality](../../../../../../triangle-inequality.md) and invariance of [Riemannian distance](../../../../../../riemannian-distance.md) under [isometries](../../../../../../isometry.md) give $d(p,\gamma p)\leq Lm$.

A [properly discontinuous group action](../../../../../../properly-discontinuous-group-action.md) has finite point stabilizer $F=\Gamma_p$ and a discrete orbit. More explicitly, properness on compact sets shows that only finitely many elements move $p$ into any bounded ball, since closed bounded balls are compact by the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md). Thus there is $\rho>0$ such that distinct orbit points have distance more than $2\rho$: choose it using the finitely many orbit points within a fixed small ball of $p$, and translate the resulting separation by [isometries](../../../../../../isometry.md). If the whole orbit is one point, the group itself is finite and the conclusion is immediate.

Let $N_m$ be the number of distinct orbit points represented by the [word metric](../../../../../../word-metric.md) ball of radius $m$. Their radius-$\rho$ balls are disjoint, have equal positive volume $v_0=\operatorname{Vol}B(p,\rho)$, and lie inside $B(p,Lm+\rho)$. The allowed [Bishop-Gromov inequality](../../../../../../bishop-gromov-inequality.md) for nonnegative [Ricci curvature](../../../../../../ricci-curvature.md) states that $\operatorname{Vol}B(p,R)/R^n$ is nonincreasing for $R>0$. Therefore

$$
N_mv_0\leq\operatorname{Vol}B(p,Lm+\rho)\leq v_0\left(\frac{Lm+\rho}{\rho}\right)^n.
$$

Each orbit point has at most $|F|$ preimages inside the word ball, since its full fiber is a coset of $F$. For the [growth function of a finitely generated group](../../../../../../growth-function-of-a-finitely-generated-group.md), this gives

$$
\boxed{\beta_\Gamma(m)\leq |F|\left(1+\frac{Lm}{\rho}\right)^n=O(m^n).}
$$

Hence $\Gamma$ has [polynomial growth of a group](../../../../../../polynomial-growth-of-a-group.md) of degree at most $n$. The finite stabilizer factor makes the proof valid even when the properly discontinuous action is not free. This is [polynomial growth of properly discontinuous isometry groups](../../../../../../polynomial-growth-of-properly-discontinuous-isometry-groups.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
