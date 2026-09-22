<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $h_i=\delta F/\delta p_i$ be the [polar molecular field](../../../../../../polar-molecular-field.md), with the positive [functional derivative](../../../../../../functional-derivative.md) convention used in the paper. During a pure advective displacement $u_j$, the [polar order parameter](../../../../../../polar-order-parameter.md) changes by

$$
\delta p_i=-u_j\partial_jp_i-\Omega^u_{ij}p_j+\xi D^u_{ij}p_j,
\quad \Omega^u_{ij}=\frac{\partial_i u_j-\partial_j u_i}{2},
\quad D^u_{ij}=\frac{\partial_i u_j+\partial_j u_i}{2}.
$$

The [free energy](../../../../../../thermodynamic-free-energy.md) change is $\delta F=\int h_i\delta p_i\,d^dr$. Assume periodic boundaries, or boundary conditions that eliminate the surface work, and [incompressibility](../../../../../../incompressible-flow.md) $\partial_j u_j=0$. [Integration by parts](../../../../../../integration-by-parts.md) in the advective term gives

$$
-\int h_i u_j\partial_jp_i\,d^dr
=\int u_jp_i\partial_jh_i\,d^dr
=\int\Sigma^{(1)}_{ij}\partial_i u_j\,d^dr,
\qquad \partial_i\Sigma^{(1)}_{ij}=-p_k\partial_jh_k.
$$

Relabelling the dummy indices in the rotational and [flow alignment of a polar order parameter](../../../../../../flow-alignment-of-a-polar-order-parameter.md) terms gives

$$
-h_i\Omega^u_{ij}p_j
=\frac{p_i h_j-p_jh_i}{2}\partial_i u_j,
\qquad
\xi h_iD^u_{ij}p_j
=\frac{\xi(p_i h_j+p_jh_i)}2\partial_i u_j.
$$

Therefore $\delta F=\int\Sigma^p_{ij}\partial_i u_j\,d^dr$, with the [reversible stress of a polar liquid crystal](../../../../../../reversible-stress-of-a-polar-liquid-crystal.md)

$$
\boxed{\Sigma^p_{ij}=\Sigma^{(1)}_{ij}
+\frac{p_i h_j-p_jh_i}{2}
+\frac{\xi(p_i h_j+p_jh_i)}2,
\quad \partial_i\Sigma^{(1)}_{ij}=-p_k\partial_jh_k}.
$$

For a local [free-energy density](../../../../../../free-energy-density.md) $f(\mathbf p,\nabla\mathbf p)$, an explicit choice is

$$
\Sigma^{(1)}_{ij}=(f-p_kh_k)\delta_{ij}
-\frac{\partial f}{\partial(\partial_i p_k)}\partial_jp_k.
$$

Its [divergence](../../../../../../divergence.md) is exactly $-p_k\partial_jh_k$, by the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) for $h_k$. A [pressure](../../../../../../pressure.md) term can be reassigned in an [incompressible flow](../../../../../../incompressible-flow.md); the chosen representative realizes the printed divergence without that ambiguity. The force density $\partial_i\Sigma^p_{ij}$ has mechanical power $-\int\Sigma^p_{ij}\partial_i v_j$, the negative of the advective [free energy](../../../../../../thermodynamic-free-energy.md) rate, which checks the stress sign.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
