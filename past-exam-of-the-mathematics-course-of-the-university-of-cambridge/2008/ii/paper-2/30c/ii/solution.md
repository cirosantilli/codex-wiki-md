<h1 id="30c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) states that if $u$ is harmonic on a neighborhood of a closed ball, then its average on the ball or its boundary sphere equals its value at the center. To prove it in three dimensions, define $M(r)=(4\pi)^{-1}\int_{S^2}u(x+r\omega)d\omega$. Differentiation and the [divergence theorem](../../../../../../divergence-theorem.md) give

$$
M'(r)=\frac1{4\pi r^2}\int_{\partial B(x,r)}\partial_nu\,dS=\frac1{4\pi r^2}\int_{B(x,r)}\Delta u\,dy=0.
$$

Since $M(r)\to u(x)$ as $r\to0$, the spherical average equals $u(x)$. Integrating $4\pi r^2M(r)$ from zero to the ball radius gives the volume version,

$$
\boxed{u(x)=\frac1{|B(x,R)|}\int_{B(x,R)}u(y)dy.}
$$

For balls merely contained in the open harmonicity domain, apply the result first to smaller radii and pass to the radius of interest by continuity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [30C](../../30c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
