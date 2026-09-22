<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [vector bundle morphism](../../../../../../vector-bundle-morphism.md) over $M$ is a smooth map $F:E\to E'$ with $\pi'\circ F=\pi$ whose restriction $E_p\to E'_p$ is linear for every $p$. A [vector bundle isomorphism](../../../../../../vector-bundle-isomorphism.md) is such a map with a smooth bundle-morphism inverse. Equivalently, a fiberwise bijective smooth bundle morphism is an isomorphism: in local [vector bundle trivializations](../../../../../../vector-bundle-trivialization.md) it is multiplication by an invertible smooth [matrix](../../../../../../matrix.md), and its inverse [matrix](../../../../../../matrix.md) is smooth.

For a [diffeomorphism](../../../../../../diffeomorphism.md) $f:N\to M$, define

$$
F:TN\longrightarrow f^*TM,\qquad v_p\longmapsto(p,df_p(v_p)).
$$

The derivative $df_p$ is a [linear isomorphism](../../../../../../linear-isomorphism.md) by the [chain rule](../../../../../../chain-rule.md), since $d(f^{-1})_{f(p)}\circ df_p=\operatorname{id}$. In [manifold charts](../../../../../../manifold-chart.md), $F$ is represented by the smooth [Jacobian matrix](../../../../../../jacobian-matrix.md) of $f$, so it is a smooth bundle morphism. Its inverse is

$$
(p,w_{f(p)})\longmapsto d(f^{-1})_{f(p)}w_{f(p)},
$$

which is also smooth and fiberwise linear. Consequently

$$
\boxed{TN\cong f^*TM\quad\text{as vector bundles over }N.}
$$

This identifies the bundles over the same base $N$; the tangent map by itself is a map from $TN$ to $TM$ covering $f$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
