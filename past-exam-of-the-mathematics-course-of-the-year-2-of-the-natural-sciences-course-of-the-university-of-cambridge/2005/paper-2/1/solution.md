<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a bounded region $R$ with piecewise smooth boundary and a continuously differentiable vector field, the [divergence theorem](../../../../divergence-theorem.md) gives $\int_R\nabla\cdot\mathbf F\,dV=\int_{\partial R}\mathbf F\cdot\mathbf n\,dS$, with outward unit normal $\mathbf n$. Apply it to $\mathbf F=u\nabla v-v\nabla u$. The cross terms cancel, giving the [Green's second identity](../../../../green-second-identity.md)

$$
\int_{B_R}[u(\Delta-m^2)v-v(\Delta-m^2)u]dV=\int_{\partial B_R}(u\partial_nv-v\partial_nu)dS.
$$

The $m^2uv$ terms cancel identically. Sending $R\to\infty$ proves the whole-space identity **provided the boundary integral tends to zero**. The [boundary term at infinity in Green's second identity](../../../../boundary-term-at-infinity-in-green-s-second-identity.md) requires adequate derivative decay as well as field decay; mere pointwise convergence $u,v\to0$ does not suffice. The screened kernels used below satisfy the required decay.

Take $m>0$. Apply the identity with $u=\phi$ and $v=G(\cdot,\mathbf r)$, treating the source through its [Dirac delta function](../../../../dirac-delta-function.md), or excising a small source sphere and taking its radius to zero. It gives $\phi(\mathbf r)-\int G(\mathbf r',\mathbf r)\rho(\mathbf r')dV'=0$. Symmetry of the radial [Green function](../../../../green-s-function-split.md) then yields the requested representation.

For separation $s=|\mathbf r-\mathbf r'|>0$, the [modified Helmholtz equation](../../../../modified-helmholtz-equation.md) reduces to $(sG)''-m^2(sG)=0$. Decay selects $G=Ce^{-ms}/s$. Integrating the equation over a small sphere gives $4\pi s^2G'\to1$, so $C=-1/(4\pi)$. Thus

$$
\boxed{G(\mathbf r,\mathbf r')=-\frac{e^{-m|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad\phi(\mathbf r)=\int G(\mathbf r,\mathbf r')\rho(\mathbf r')dV'.}
$$

For $\rho=e^{-\beta r}/r$ with $\beta>0$, put $h=r\phi$. Then $h''-m^2h=e^{-\beta r}$. When $\beta\ne m$, decay removes $e^{mr}$, while $h(0)=0$ removes an additional point source at the origin. Hence

$$
\boxed{\phi(r)=\frac{e^{-\beta r}-e^{-mr}}{r(\beta^2-m^2)}.}
$$

Since $G$ has a minus sign, the positive [Yukawa kernel convolution](../../../../yukawa-kernel-convolution.md) is

$$
\boxed{\frac1{4\pi}\int_{\mathbb R^3}\frac{e^{-m|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}\frac{e^{-\beta r'}}{r'}dV'=-\frac{e^{-\beta r}-e^{-mr}}{r(\beta^2-m^2)}.}
$$

The coincident-rate limit $\beta=m$ is $e^{-mr}/(2m)$ for the convolution, and the origin limit for general rates is $1/(m+\beta)$. Both are finite; the apparent denominators in the distinct-rate formula are removable limits.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
