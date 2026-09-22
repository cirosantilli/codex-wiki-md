<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mu:P\to\mathbb R$ be the [moment map](../../../../../../moment-map.md) for the [circle group](../../../../../../circle-group.md), assume $c$ is a [regular value](../../../../../../regular-value.md), and assume the circle action on $N=\mu^{-1}(c)$ is free. The action is proper because the circle is compact. Then $N$ has dimension $2n-1$ and $P_c=N/SO(2)$ is a smooth [manifold](../../../../../../topological-manifold.md) of dimension $2n-2$.

If $\xi_P$ generates the action, $\omega(\xi_P,v)=d\mu(v)=0$ for every $v\in TN$. In fact $(TN)^\omega$ is exactly the line spanned by $\xi_P$, since $TN=\ker d\mu$ is a hyperplane and $\omega$ is nondegenerate. Therefore the kernel of the restricted two-form is precisely the orbit direction. The restriction is invariant and horizontal, so it descends to a unique nondegenerate closed two-form $\omega_c$ with

$$
\boxed{\pi^*\omega_c=\iota^*\omega.}
$$

This proves the [Marsden-Weinstein theorem](../../../../../../marsden-weinstein-theorem.md) in the circle case. If the [Hamiltonian](../../../../../../hamiltonian.md) $H$ is invariant, then $\{\mu,H\}=0$: its [Hamiltonian flow](../../../../../../hamiltonian-flow.md) stays on $N$, projects to the quotient and is generated there by the descended function $H_c$. This is a reduced [Hamiltonian system](../../../../../../hamiltonian-system.md) in $2n-2$ local variables. At a critical level or a nonfree orbit the quotient can be singular, so the smooth dimension assertion needs the stated hypotheses.

For a mass-$m$ particle in the plane with [central force](../../../../../../central-force.md) potential $V(r)$, work on $r>0$ and write

$$
p_xdx+p_ydy=p_rdr+\ell d\theta,\quad
p_r=\frac{xp_x+yp_y}{r},\quad \ell=xp_y-yp_x.
$$

Exterior differentiation gives $\omega=dr\wedge dp_r+d\theta\wedge d\ell$. Rotation translates $\theta$ and has [moment map](../../../../../../moment-map.md) $\ell$. Fix $\ell=\ell_0$ and quotient out $\theta$ to obtain the [planar rotational symplectic reduction](../../../../../../planar-rotational-symplectic-reduction.md)

$$
\boxed{\omega_{\mathrm{red}}=dr\wedge dp_r,\qquad
H_{\mathrm{red}}=\frac{p_r^2}{2m}+\frac{\ell_0^2}{2mr^2}+V(r).}
$$

The reduced equations are $\dot r=p_r/m$ and $\dot p_r=\ell_0^2/(mr^3)-V'(r)$. The centrifugal term arises from the conserved angular momentum; it is not an extra force imposed by hand. Reconstruct the angle from $\dot\theta=\ell_0/(mr^2)$. For $\ell_0\ne0$ the origin cannot lie on the level; for $\ell_0=0$ the same local reduction holds away from the origin, while the full phase-space origin is a singular fixed orbit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
