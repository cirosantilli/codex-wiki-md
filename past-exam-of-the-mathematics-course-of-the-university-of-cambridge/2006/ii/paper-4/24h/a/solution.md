<h1 id="24h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $J$ be rotation by ninety degrees in the oriented tangent plane, $Jv=N\times v$. In local coordinates seek a curve with

$$
\nabla_{\dot\gamma}\dot\gamma=\lambda J\dot\gamma,
\quad\text{or}\quad
\ddot x^k+\Gamma^k_{ij}\dot x^i\dot x^j=\lambda J^k_i\dot x^i.
$$

This smooth second-order [ordinary differential equation](../../../../../../ordinary-differential-equation.md), written as a first-order system for $(x,\dot x)$, has a unique local solution with the specified initial position and velocity. Its speed is constant, since

$$
\frac d{dt}|\dot\gamma|^2=2\langle\nabla_{\dot\gamma}\dot\gamma,\dot\gamma\rangle
=2\lambda\langle J\dot\gamma,\dot\gamma\rangle=0.
$$

The initial speed is one, so the parameter is arc-length and the signed [geodesic curvature](../../../../../../geodesic-curvature.md) is $\langle\nabla_s\dot\gamma,J\dot\gamma\rangle=\lambda$. Conversely every requested curve satisfies this system, which proves the claimed uniqueness as well as existence on some $(-\epsilon,\epsilon)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24H](../../24h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
