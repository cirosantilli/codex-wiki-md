<h1 id="26g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The induced metric makes the compact surface $S$ a compact Riemannian manifold. By the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md) it is geodesically complete, so every $\exp_p$ is defined on all of $T_pS$. In particular, $\exp_p(V(p))$ is defined for every $p$.

The global exponential map

$$
\operatorname{Exp}:TS\to S,
\qquad (p,v)\mapsto\exp_p(v),
$$

is smooth by smooth dependence of geodesics on initial data. Since $p\mapsto(p,V(p))$ is a smooth section of $TS$, their composition

$$
\phi(p)=\operatorname{Exp}(p,V(p))
$$

is smooth.

For $0\leq t\leq1$, define

$$
\phi_t(p)=\exp_p(tV(p)).
$$

Completeness makes this a well-defined smooth homotopy, with $\phi_0=\operatorname{id}_S$ and $\phi_1=\phi$. By homotopy invariance of [degree modulo two](../../../../../../degree-modulo-two.md),

$$
\deg_2(\phi)=\deg_2(\operatorname{id}_S)=1.
$$

This is the [exponential displacement map on a compact surface](../../../../../../exponential-displacement-map-on-a-compact-surface.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [26G](../../26g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
