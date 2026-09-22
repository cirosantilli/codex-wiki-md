<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

For a nonconstant [holomorphic map](../../../../../holomorphic-map.md) $f:X\to Y$ between compact connected [Riemann surfaces](../../../../../riemann-surfaces.md), its [degree](../../../../../degree-of-a-holomorphic-map.md) is

$$
\deg f=\sum_{x\in f^{-1}(y)}e_x,
$$

where $e_x$ is the [ramification index of a holomorphic map](../../../../../ramification-index-of-a-holomorphic-map.md) at $x$. The [valency theorem](../../../../../valency-theorem.md) makes this sum independent of $y\in Y$. The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) is

$$
\boxed{2g_X-2=(\deg f)(2g_Y-2)+\sum_{x\in X}(e_x-1).}
$$

Write $E=\mathbb C/\Lambda$. The map $\psi(z+\Lambda)=-z+\Lambda$ is well-defined and [biholomorphic](../../../../../biholomorphism.md), with $\psi^2=\operatorname{id}$. Its fixed points satisfy

$$
z+\Lambda=-z+\Lambda
\iff2z\in\Lambda.
$$

They are therefore indexed by $\tfrac12\Lambda/\Lambda\cong(\mathbb Z/2\mathbb Z)^2$, so there are four, as in the [negation map on a one-dimensional complex torus](../../../../../negation-map-on-a-one-dimensional-complex-torus.md).

For each $x\in E'$ choose a small open disc $U_x$ for which $U_x\cap\psi(U_x)=\varnothing$. The projection restricts to a homeomorphism

$$
p|_{U_x}:U_x\longrightarrow p(U_x).
$$

Use $(p|_{U_x})^{-1}$ followed by a holomorphic coordinate on $U_x$ as a chart on $p(U_x)$. Choosing $\psi(U_x)$ instead changes this coordinate by the holomorphic map induced by $\psi$, so the transition functions are holomorphic. These charts make $S'$ a [Riemann surface](../../../../../riemann-surfaces.md) and $p:E'\to S'$ a holomorphic double [covering map](../../../../../covering-space.md).

At each omitted fixed point, a centred local coordinate changes by $z\mapsto-z$, so the invariant quotient coordinate is $w=z^2$. Hence the extension has degree two and exactly four ramification points, each with $e_x=2$. Since the [complex torus](../../../../../complex-torus.md) $E$ has genus one, [Riemann--Hurwitz](../../../../../riemann-hurwitz-formula.md) gives

$$
0=2(2g_S-2)+4.
$$

Thus **$\boxed{g_S=0}$**, in agreement with the general [quotient of a one-dimensional complex torus by negation](../../../../../quotient-of-a-one-dimensional-complex-torus-by-negation.md).

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
