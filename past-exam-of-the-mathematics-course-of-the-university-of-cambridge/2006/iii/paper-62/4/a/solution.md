<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At [linear order](../../../../../../linear-order.md) a coordinate displacement $\xi^\mu$ changes a [metric perturbation](../../../../../../linearized-gravity.md) by $q_{\mu\nu}\mapsto q_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}$. Work in [conformal time](../../../../../../conformal-time.md) with $\bar g_{\mu\nu}=a^2\operatorname{diag}(-1,1,1,1)$, write $\xi^0=\alpha$ and lower spatial indices with $\delta_{ij}$. Directly evaluating the [Lie derivative of a covariant tensor field](../../../../../../lie-derivative-of-a-covariant-tensor-field.md) gives

$$
q'_{00}=q_{00}+2a^2(\alpha'+\mathcal H\alpha),\qquad q'_{0i}=q_{0i}-a^2(\xi_i'-\partial_i\alpha),\qquad\mathcal H=\frac{a'}a.
$$

Here primes on $\alpha,\xi_i$ mean conformal-time derivatives, while primes on $q'_{0\mu}$ label transformed components. Setting the transformed lapse and shift perturbations to zero requires

$$
\alpha'+\mathcal H\alpha=-\frac{q_{00}}{2a^2},\qquad \xi_i'=\frac{q_{0i}}{a^2}+\partial_i\alpha.
$$

These are first-order time equations. Their explicit local solutions are

$$
\alpha(\tau,x)=\frac1{a(\tau)}\left[C(x)-\int^{\tau}\frac{q_{00}(s,x)}{2a(s)}\,ds\right],\qquad
\xi_i(\tau,x)=D_i(x)+\int^{\tau}\left[\frac{q_{0i}(s,x)}{a(s)^2}+\partial_i\alpha(s,x)\right]ds.
$$

Thus four coordinate functions can impose the four synchronous conditions in any regular perturbative patch. This is [synchronous gauge fixing by coordinate displacement](../../../../../../synchronous-gauge-fixing-by-coordinate-displacement.md). The arbitrary spatial functions $C,D_i$ remain as residual gauge freedom; the conditions alone do not fix the coordinate system completely.

Geometrically, synchronous coordinates follow a congruence of freely falling observers launched normally from a spatial slice, using their [proper time](../../../../../../proper-time.md). This gives unit lapse and zero shift in [cosmic time](../../../../../../cosmic-time.md); conversion to background [conformal time](../../../../../../conformal-time.md) gives the displayed convention. “Always possible” is local: [geodesic](../../../../../../geodesic.md) caustics or singularities can prevent a global synchronous chart. Such global obstructions do not invalidate local [linear cosmological perturbation theory](../../../../../../linear-cosmological-perturbation-theory-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
