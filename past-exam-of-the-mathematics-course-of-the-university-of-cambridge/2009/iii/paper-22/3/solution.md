<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the positive [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) on a compact [Riemannian manifold](../../../../../riemannian-manifold.md) without boundary. Its [heat kernel](../../../../../heat-kernel.md) is the smooth integral kernel $K(t,x,y)$, $t>0$, of the solution operators for the [heat equation](../../../../../heat-equation.md):

$$
(\partial_t+\Delta_x)K=0,\qquad
u(t,x)=\int_MK(t,x,y)f(y)\,dV_g(y),\qquad
u(t,\cdot)\longrightarrow f\quad(t\downarrow0).
$$

The last condition holds, in particular, in $L^2$ for smooth initial functions. The [heat trace](../../../../../heat-trace.md) is

$$
Z_M(t)=\operatorname{Tr}(e^{-t\Delta})=\int_MK(t,x,x)\,dV_g(x).
$$

The [heat invariants](../../../../../heat-invariants.md) are the coefficients in the small-time [heat kernel expansion](../../../../../heat-kernel-expansion.md) of this trace:

$$
Z_M(t)\sim(4\pi t)^{-d/2}\sum_{j=0}^\infty a_jt^j,
\qquad a_0=\operatorname{Vol}(M),\quad
 a_1=\frac16\int_M R_g\,dV_g.
$$

Equivalently, the local diagonal coefficients $u_j(x,x)$ integrate to $a_j$; $R_g$ is the [scalar curvature](../../../../../scalar-curvature.md). Some normalizations absorb $(4\pi)^{-d/2}$ into the coefficients. These definitions here use the displayed normalization consistently.

To prove uniqueness, let $K_1,K_2$ satisfy the [heat kernel](../../../../../heat-kernel.md) conditions and let $w$ be the difference of their solutions with the same smooth initial function. It solves $w_t=-\Delta w$ and tends to zero in $L^2$ as $t\downarrow0$. The [heat equation energy identity](../../../../../heat-equation-energy-identity.md), using [integration by parts](../../../../../integration-by-parts.md) on the closed manifold, gives for $t>0$

$$
\frac{d}{dt}\|w(t)\|_{L^2}^2
=-2\langle\Delta w,w\rangle_{L^2}
=-2\int_M|dw|_g^2\,dV_g\leq0.
$$

Integrating from $s>0$ to $t$ gives $\|w(t)\|_{L^2}\leq\|w(s)\|_{L^2}$; sending $s\downarrow0$ proves $w(t)=0$. Thus for every smooth test function $f$,

$$
\int_M(K_1-K_2)(t,x,y)f(y)\,dV_g(y)=0.
$$

For fixed positive $t$ and $x$, smoothness makes this difference a smooth function of $y$. Taking its conjugate as test function shows its squared norm is zero. **The heat kernel is unique.**

The [compact elliptic spectral theorem](../../../../../compact-elliptic-spectral-theorem.md) for the [self-adjoint](../../../../../self-adjoint-operator.md) elliptic [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) gives a complete orthonormal [basis](../../../../../basis.md) of smooth [eigenfunctions](../../../../../eigenfunction.md) $\phi_j$, with discrete [eigenvalues](../../../../../eigenvalue.md) $0\leq\lambda_0\leq\lambda_1\leq\cdots$ counted with multiplicity. Solving the [heat equation](../../../../../heat-equation.md) for initial data $\phi_j$ gives $e^{-t\lambda_j}\phi_j$, so the unique [heat kernel](../../../../../heat-kernel.md) has its [eigenfunction expansion](../../../../../eigenfunction-expansion.md) and its [heat trace](../../../../../heat-trace.md) is

$$
\boxed{Z_M(t)=\sum_j e^{-t\lambda_j}.}
$$

The series converges for every $t>0$. This proves that the [spectrum](../../../../../spectrum-functional-analysis.md) with multiplicities determines the [heat trace](../../../../../heat-trace.md).

Conversely, its large-time behaviour recovers the distinct [eigenvalues](../../../../../eigenvalue.md) and their multiplicities successively. The multiplicity of zero is $m_0=\lim_{t\to\infty}Z_M(t)$. After subtracting the already determined terms, let

$$
R(t)=Z_M(t)-\sum_{\nu<\mu}m_\nu e^{-t\nu}
$$

be the positive remaining sum, and let $\mu$ be its smallest remaining [eigenvalue](../../../../../eigenvalue.md). Then

$$
\boxed{\mu=-\lim_{t\to\infty}\frac{\log R(t)}t,\qquad
m_\mu=\lim_{t\to\infty}e^{t\mu}R(t).}
$$

Indeed, after factoring $e^{-t\mu}$, the next distinct [eigenvalue](../../../../../eigenvalue.md) is separated from $\mu$ by a positive gap. The remaining tail tends to zero: for fixed $t_0>0$ its absolute sum is bounded by a constant times $e^{-(\mu_{\mathrm{next}}-\mu)(t-t_0)}$, using finiteness of $Z_M(t_0)$. Induction recovers every spectral term. Thus **the heat trace and the spectrum with multiplicities determine one another**.

Finally the leading coefficient among the [heat invariants](../../../../../heat-invariants.md) is positive, so

$$
\boxed{d=2\lim_{t\downarrow0}\frac{\log Z_M(t)}{\log(1/t)}.}
$$

The common [heat trace](../../../../../heat-trace.md) of [isospectral manifolds](../../../../../isospectral-manifolds.md) therefore forces them to have the same dimension. Once the dimension is recovered, its leading coefficient also recovers their common volume.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
