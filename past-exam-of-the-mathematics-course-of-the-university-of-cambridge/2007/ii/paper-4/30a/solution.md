<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

For a $C^2$ function, let $M(r)=(4\pi)^{-1}\int_{S^2}u(y+r\omega)\,d\omega$ be its spherical mean. Differentiation and the [divergence theorem](../../../../../divergence-theorem.md) give

$$
M'(r)=\frac1{4\pi r^2}\int_{\partial B(y,r)}\partial_nu\,dS
=\frac1{4\pi r^2}\int_{B(y,r)}\Delta u\,dx.
$$

If $u$ is harmonic, this derivative is zero; since $M(0)=u(y)$ by continuity, **every spherical mean equals the value at the centre**. Integrating $4\pi r^2M(r)$ over $0<r<R$ gives the same statement for the volume mean on a ball. This proves the [mean value property for harmonic functions](../../../../../mean-value-property-for-harmonic-functions.md).

If $u$ is subharmonic, $\Delta u\geq0$, so $M'(r)\geq0$. Thus

$$
\boxed{u(y)\leq\frac1{|\partial B(y,R)|}\int_{\partial B(y,R)}u\,dS,
\qquad u(y)\leq\frac1{|B(y,R)|}\int_{B(y,R)}u\,dx.}
$$

These are the corresponding mean value inequalities. A [subharmonic function](../../../../../subharmonic-function.md) has the maximum principle on a ball: apply the second-derivative test to $u+\epsilon|x-y|^2$, whose Laplacian is strictly positive and hence cannot have an interior maximum, then let $\epsilon\downarrow0$.

For $w=|\phi|^2$, the given equation says $\Delta\phi=iV\phi$. Since $V$ is real,

$$
\Delta w=2|\nabla\phi|^2+2\operatorname{Re}(\overline\phi\Delta\phi)
=2|\nabla\phi|^2\geq0.
$$

The subharmonic maximum principle gives $w(x)\leq\max_{\partial B}w$ throughout the ball. Taking square roots yields

$$
\boxed{\sup_{B(y,R)}|\phi|\leq\sup_{\partial B(y,R)}|\phi|.}
$$

No sign condition on the real potential $V$ is needed.

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
