<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $T=T_s+T_u$. The transient satisfies the [heat equation](../../../../../../../heat-equation.md) and homogeneous mixed [boundary conditions](../../../../../../../boundary-condition.md)

$$
(T_u)_t=k(T_u)_{xx},\qquad
(T_u)_x(0,t)=0,\qquad T_u(2\ell,t)=0,\qquad
T_u(x,0)=-\frac Qk(2\ell-x).
$$

The left condition is a [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) and the right one a [Dirichlet boundary condition](../../../../../../../dirichlet-boundary-condition.md). [Separation of variables](../../../../../../../separation-of-variables.md), $T_u=X(x)G(t)$, gives

$$
\frac{G'}{kG}=\frac{X''}{X}=-\mu^2,\qquad
X''+\mu^2X=0,\qquad G=e^{-k\mu^2t}.
$$

The condition $X'(0)=0$ removes the [sine](../../../../../../../sine.md) term. The condition $X(2\ell)=0$ then selects

$$
\mu_n=\frac{(2n+1)\pi}{4\ell},\qquad
X_n(x)=\cos(\mu_nx),\qquad n=0,1,2,\ldots.
$$

There is no nonzero mode with $\mu=0$, because a linear $X$ satisfying both conditions is zero. There is no growing mode either: [integration by parts](../../../../../../../integration-by-parts.md) gives $\int_0^{2\ell}(X')^2dx=\mu^2\int_0^{2\ell}X^2dx$, so every nonzero mode has $\mu^2>0$.

These [Sturm-Liouville eigenfunctions](../../../../../../../sturm-liouville-eigenfunction.md) have [orthogonality](../../../../../../../orthogonal-vectors.md) and squared [norm](../../../../../../../norm.md)

$$
\int_0^{2\ell}\cos(\mu_nx)\cos(\mu_jx)\,dx=\ell\,\delta_{nj}.
$$

Expand the initial transient in this half-integer [Fourier cosine series](../../../../../../../fourier-cosine-series.md). Its coefficients are

$$
\begin{aligned}
A_n&=-\frac Q{k\ell}\int_0^{2\ell}(2\ell-x)\cos(\mu_nx)\,dx\\
&=-\frac Q{k\ell}\frac{1-\cos(2\ell\mu_n)}{\mu_n^2}
=-\frac{16Q\ell}{k\pi^2(2n+1)^2}.
\end{aligned}
$$

The integration formula follows by [integration by parts](../../../../../../../integration-by-parts.md); the cosine at the endpoint is zero. Thus the [half-integer cosine expansion of a linear profile](../../../../../../../half-integer-cosine-expansion-of-a-linear-profile.md) gives

$$
\boxed{T(x,t)=\frac Qk(2\ell-x)
-\frac{16Q\ell}{k\pi^2}\sum_{n=0}^\infty
\frac{\cos\!\left(\frac{(2n+1)\pi x}{4\ell}\right)}{(2n+1)^2}
\exp\!\left(-\frac{(2n+1)^2\pi^2kt}{16\ell^2}\right).}
$$

At $t=0$ the [Fourier series](../../../../../../../fourier-series-split.md) reproduces $-T_s$ everywhere, including the endpoints; its $n^{-2}$ coefficient decay gives [uniform convergence](../../../../../../../uniform-convergence.md). For every $t>0$ the exponential factors allow termwise differentiation and verify the [heat equation](../../../../../../../heat-equation.md) and both [boundary conditions](../../../../../../../boundary-condition.md). The sudden switch-on of nonzero [heat flux](../../../../../../../heat-flux-density.md) is incompatible with the spatial derivative of the constant initial temperature at the corner $(0,0)$. Accordingly, the positive-time boundary derivative must not be inferred by differentiating the initial [Fourier series](../../../../../../../fourier-series-split.md) term by term at that corner.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
