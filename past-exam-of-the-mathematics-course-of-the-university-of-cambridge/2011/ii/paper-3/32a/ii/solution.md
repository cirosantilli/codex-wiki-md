<h1 id="32a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $U,V$ depend only on $x=\rho+\tau$, then $\partial_\rho=\partial_\tau=\partial_x$ on them. Put $A=U-V$ and $B=U+V$. The curvature equation gives

$$
A'=-[U,V]=\tfrac12[A,B].
$$

By cyclicity of [matrix trace](../../../../../../matrix-trace.md),

$$
\frac d{dx}\operatorname{tr}(A^p)=p\operatorname{tr}(A^{p-1}A')=\frac p2\operatorname{tr}(A^{p-1}[A,B])=0.
$$

This is an [Isospectral Lax equation](../../../../../../isospectral-lax-equation.md) expressed as a [Lax equation](../../../../../../isospectral-lax-equation.md), and it proves the assertion for every positive integer $p$.

For the given matrices and $\phi=\phi(x)$,

$$
A=i\left[\frac{\phi'}2\sigma_1+\frac{\sin\phi}{4\lambda}\sigma_2+\left(\lambda+\frac{\cos\phi}{4\lambda}\right)\sigma_3\right].
$$

Using $(a\cdot\sigma)^2=(a\cdot a)I$ gives

$$
\operatorname{tr}(A^2)=-2\left[\frac{(\phi')^2}{4}+\lambda^2+\frac{\cos\phi}{2}+\frac1{16\lambda^2}\right].
$$

Since $\lambda$ is fixed, constancy of this trace yields the [first integral](../../../../../../first-integral.md)

$$
\boxed{\frac12(\phi')^2+\cos\phi=C.}
$$

Differentiating confirms $dC/dx=\phi'(\phi''-\sin\phi)=0$ for the reduced equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [32A](../../32a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
