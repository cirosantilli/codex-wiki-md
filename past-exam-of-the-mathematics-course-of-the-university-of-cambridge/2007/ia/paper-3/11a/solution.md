<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

For a real-valued function on a bounded regular region, apply the [divergence theorem](../../../../../divergence-theorem.md) to $\phi\nabla\phi$. The [product rule](../../../../../product-rule.md) yields $\nabla\cdot(\phi\nabla\phi)=|\nabla\phi|^2+\phi\nabla^2\phi$. The prescribed zero boundary values and [Laplace equation](../../../../../laplace-equation.md) therefore imply

$$
\int_V|\nabla\phi|^2dV=\int_{\partial V}\phi\,\partial_n\phi\,dS-\int_V\phi\nabla^2\phi\,dV=0.
$$

The continuous nonnegative integrand must vanish everywhere. Hence $\phi$ is constant on each connected component, and its boundary value makes each constant zero. This proves [zero-boundary harmonic uniqueness](../../../../../zero-boundary-harmonic-uniqueness.md). If complex-valued functions are allowed, apply the same argument separately to their real and imaginary parts. If $\psi_1,\psi_2$ solve the same [Poisson equation](../../../../../poisson-equation.md) and [Dirichlet boundary data](../../../../../dirichlet-boundary-data.md), their difference is harmonic with zero boundary value, so is zero. Thus **there is at most one solution**. An exterior unbounded region would require an additional condition at infinity; the preceding bounded-domain proof does not assert uniqueness without one.

For the radial calculation use Cartesian coordinates with $r=(x_ix_i)^{1/2}>0$. The [chain rule](../../../../../chain-rule.md) gives $\partial_ir=x_i/r$ and

$$
\boxed{\nabla\psi=\frac{\psi'(r)}r\mathbf x.}
$$

Differentiate again and sum the three coordinates:

$$
\begin{aligned}
\nabla^2\psi&=\partial_i\left(\psi'(r)\frac{x_i}r\right)\\
&=\psi''(r)\frac{x_ix_i}{r^2}+\psi'(r)\left(\frac3r-\frac{x_ix_i}{r^3}\right)\\
&=\psi''(r)+\frac2r\psi'(r)=\boxed{\frac1r\frac{d^2(r\psi)}{dr^2}}.
\end{aligned}
$$

This derives the [radial Laplacian](../../../../../radial-laplacian.md) directly in Cartesian coordinates. For $\nabla^2\psi=c$, set $u=r\psi$, so $u''=cr$. Integrating twice gives $u=cr^3/6+ar+b$, and consequently

$$
\boxed{\psi(r)=\frac{cr^2}{6}+a+\frac br,\qquad r>0.}
$$

If the solution must extend boundedly through the origin, $b=0$. The remaining polynomial is smooth there.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
