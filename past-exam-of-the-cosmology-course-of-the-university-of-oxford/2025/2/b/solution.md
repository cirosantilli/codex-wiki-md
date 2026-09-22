<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the source's $+---$ [metric signature](../../../../metric-signature.md) and $x^0=\eta$, with [conformal time](../../../../conformal-time.md) [derivatives](../../../../derivative.md) denoted by primes. For this [vector cosmological perturbation](../../../../vector-cosmological-perturbation.md), the [metric tensor](../../../../metric-tensor.md) and [inverse metric](../../../../inverse-metric.md) through first order are

$$
g_{00}=a^2,\quad g_{0i}=0,\quad g_{ij}=-a^2(\delta_{ij}-J_{ij}),\qquad
g^{00}=a^{-2},\quad g^{0i}=0,\quad g^{ij}=-a^{-2}(\delta_{ij}+J_{ij}).
$$

Spatial indices on perturbations are raised with the background [Kronecker delta](../../../../kronecker-delta.md). The [Christoffel symbol](../../../../christoffel-symbol.md) formula is

$$
\Gamma^\alpha_{\beta\gamma}=\frac12g^{\alpha\sigma}(\partial_\beta g_{\sigma\gamma}+\partial_\gamma g_{\sigma\beta}-\partial_\sigma g_{\beta\gamma}).
$$

Because $a=a(\eta)$ only, it gives

$$
\boxed{\Gamma^0_{00}=\frac12a^{-2}(2aa')=\mathcal H,\qquad \Gamma^0_{0i}=\frac12a^{-2}\partial_i(a^2)=0.}
$$

For the other requested [Christoffel symbols](../../../../christoffel-symbol.md), only the time [derivative](../../../../derivative.md) of the spatial [metric tensor](../../../../metric-tensor.md) contributes:

$$
\Gamma^0_{ij}=-\frac12a^{-2}\partial_\eta g_{ij}
=\frac12a^{-2}\left[2aa'(\delta_{ij}-J_{ij})-a^2J'_{ij}\right].
$$

Thus

$$
\boxed{\Gamma^0_{ij}=\mathcal H(\delta_{ij}-J_{ij})-\frac12J'_{ij}.}
$$

Finally contract the first upper and first lower spatial indices, summing over $i$:

$$
\gamma^i_{ij}=\frac12(\partial_iJ_{ij}+\partial_jJ_{ii}-\partial_iJ_{ij})=\frac12\partial_jJ_{ii}.
$$

Since $J_{ii}=2\partial_iF_i=0$ by the [transverse vector field](../../../../transverse-vector-field.md) condition on $\mathbf F$,

$$
\boxed{\gamma^i_{ij}=0.}
$$

The useful [Christoffel symbol](../../../../christoffel-symbol.md) traces are consequently $\Gamma^\mu_{\mu0}=4\mathcal H$ and $\Gamma^\mu_{\mu j}=0$ to first order: the first uses $J'_{ii}=0$ and the second uses the contraction just proved.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the cosmology course of the University of Oxford](../../../split.md)
5. [Cosmology course of the University of Oxford](../../../../cosmology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
