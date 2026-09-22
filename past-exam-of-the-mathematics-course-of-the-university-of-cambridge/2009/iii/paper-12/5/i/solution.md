<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $B_r(x_0)$ have closure contained in the domain of a [harmonic function](../../../../../../harmonic-function.md) $u$. Put $\omega_n=|B_1(0)|$, so $|B_r|=\omega_nr^n$ and $|\partial B_r|=n\omega_nr^{n-1}$. The sphere and ball [mean value properties for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) are

$$
\boxed{u(x_0)=\frac1{|\partial B_r|}\int_{\partial B_r(x_0)}u\,dS=\frac1{|B_r|}\int_{B_r(x_0)}u\,dx.}
$$

To prove the sphere formula, define its average using a fixed unit sphere:

$$
M(r)=\frac1{n\omega_n}\int_{S^{n-1}}u(x_0+r\theta)\,dS_\theta.
$$

Differentiating under the integral and applying the [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
M'(r)=\frac1{n\omega_nr^{n-1}}\int_{\partial B_r(x_0)}\partial_\nu u\,dS=\frac1{n\omega_nr^{n-1}}\int_{B_r(x_0)}\Delta u\,dx=0.
$$

Continuity gives $M(r)\to u(x_0)$ as $r\downarrow0$, proving the spherical average identity. Integrating that identity over radii with the polar-coordinate weight yields

$$
\int_{B_r(x_0)}u=\int_0^r n\omega_nt^{n-1}M(t)\,dt=\omega_nr^n u(x_0),
$$

which proves the ball identity. For $n=1$, the sphere average is the average of the two endpoints, and the same formulas hold with the counting surface measure.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
