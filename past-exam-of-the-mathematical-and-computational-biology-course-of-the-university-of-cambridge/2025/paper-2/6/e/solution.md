<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Factor the [characteristic polynomial](../../../../../characteristic-polynomial.md) as $\lambda^2(\lambda^2-3)$. The [eigenvalues](../../../../../eigenvalue.md), with algebraic multiplicity, are therefore

$$
\boxed{\sqrt3,\ -\sqrt3,\ 0,\ 0}.
$$

The [adjacency matrix](../../../../../adjacency-matrix.md) describes a [star graph](../../../../../star-graph-theory.md) with node 1 as the hub. For the positive leading [eigenvalue](../../../../../eigenvalue.md) $\lambda=\sqrt3$, write the hub component as $h$. The leaf equations $h=\lambda v_i$, for $i=2,3,4$, give equal leaf components $\ell=h/\sqrt3$. The hub equation is $3\ell=\lambda h$, which is consistent precisely because $\lambda^2=3$. Thus an [eigenvector](../../../../../eigenvector.md) is $(\sqrt3,1,1,1)^\mathsf T$.

Normalizing its [Euclidean norm](../../../../../euclidean-norm.md) to one gives the [eigenvector centrality](../../../../../eigenvector-centrality.md)

$$
\boxed{v=\frac1{\sqrt6}(\sqrt3,1,1,1)^\mathsf T=\left(\frac1{\sqrt2},\frac1{\sqrt6},\frac1{\sqrt6},\frac1{\sqrt6}\right)^\mathsf T}.
$$

Numerically this is $(0.707107,0.408248,0.408248,0.408248)^\mathsf T$. It satisfies both $Av=\sqrt3v$ and $v^\mathsf Tv=1$. If “normalized” instead means maximum component one, use $(1,1/\sqrt3,1/\sqrt3,1/\sqrt3)$; if it means components summing to one, divide $(\sqrt3,1,1,1)$ by $\sqrt3+3$. The hub-to-leaf ratio $\sqrt3$ is invariant under these conventions. The negative leading-magnitude [eigenvalue](../../../../../eigenvalue.md) also has an [eigenvector](../../../../../eigenvector.md), but its mixed signs do not define nonnegative [eigenvector centrality](../../../../../eigenvector-centrality.md).

## ↑ Ancestors (13)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
