<h1 id="26g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $v\in T_pS$, let $\gamma_v$ be the maximal [geodesic](../../../../../../geodesic.md) satisfying

$$
\gamma_v(0)=p,
\qquad
\dot\gamma_v(0)=v.
$$

The [exponential map](../../../../../../exponential-map-riemannian-geometry.md) is

$$
\exp_p(v)=\gamma_v(1)
$$

on the [domain of the exponential map](../../../../../../domain-of-the-exponential-map.md)

$$
\mathcal D_p
=\{v\in T_pS:\gamma_v\text{ is defined throughout }[0,1]\}.
$$

This is an open, star-shaped neighbourhood of zero. In local coordinates the geodesic equation is a smooth ordinary differential equation, so smooth dependence on its initial position and velocity proves that $(p,v)\mapsto\exp_p(v)$ is smooth on its domain.

For both requested phenomena consider the embedded surface

$$
S=\{(x,y,0):(x,y)\ne(0,0)\}
$$

with $p=(1,0,0)$. Its geodesics are Euclidean straight lines for as long as they remain in $S$. The initial vector $v=(-2,0,0)$ would give

$$
\gamma_v(t)=(1-2t,0,0),
$$

which reaches the missing origin at $t=1/2$. Thus $v\notin\mathcal D_p$, and the domain is not all of $T_pS$.

The point $q=(-1,0,0)$ is not in the image of $\exp_p$. Any geodesic from $p$ to $q$ would have to be their unique Euclidean straight line, which passes through the omitted origin. Hence this exponential map is also not surjective, as summarized by [exponential map of the punctured plane](../../../../../../exponential-map-of-the-punctured-plane.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
