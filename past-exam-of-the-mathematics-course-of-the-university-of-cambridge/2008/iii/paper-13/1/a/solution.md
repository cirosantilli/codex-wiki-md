<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\omega_n=|B_1|$. If $u$ is a $C^2$ [harmonic function](../../../../../../harmonic-function.md) and $\overline{B_r(x)}\subset\Omega$, its two [mean value properties for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) are

$$
\boxed{u(x)=\frac1{n\omega_n r^{n-1}}\int_{\partial B_r(x)}u\,dS
=\frac1{\omega_n r^n}\int_{B_r(x)}u\,dy.}
$$

To prove the spherical property, express the normalized spherical mean on the fixed unit sphere:

$$
M(r)=\frac1{n\omega_n}\int_{S^{n-1}}u(x+r\theta)\,dS_\theta.
$$

Differentiation and the [divergence theorem](../../../../../../divergence-theorem.md) give

$$
M'(r)=\frac1{n\omega_n r^{n-1}}\int_{\partial B_r(x)}\partial_\nu u\,dS
=\frac1{n\omega_n r^{n-1}}\int_{B_r(x)}\Delta u\,dy=0.
$$

Since [continuity](../../../../../../continuous-function.md) gives $M(r)\to u(x)$ as $r\downarrow0$, the spherical mean equals $u(x)$ for every admissible radius. Integrate this identity in radial coordinates:

$$
\int_{B_r(x)}u\,dy=n\omega_n\int_0^r t^{n-1}M(t)\,dt=\omega_n r^n u(x).
$$

This proves the ball mean property as well. For $n=1$, the sphere consists of the two endpoints and the same argument is the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
