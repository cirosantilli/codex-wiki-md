<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take the difference $w$ of two solutions with the same [body force](../../../../../body-force.md), initial displacement and initial [velocity](../../../../../velocity.md). It satisfies the homogeneous [linear elasticity](../../../../../linear-elasticity.md) equations. With $e=e(w)$ the [infinitesimal strain tensor](../../../../../infinitesimal-strain-tensor.md), define the bulk [energy](../../../../../energy.md)

$$
E_{\rm bulk}(t)=\frac12\int_D\{\rho|w_t|^2+C_{ijkl}e_{ij}e_{kl}\}\,dV.
$$

The usual stability assumptions make the elastic quadratic form nonnegative and $\rho>0$. Multiplying momentum balance by $w_t$, using [integration by parts](../../../../../integration-by-parts.md) and using symmetry of the [stress tensor](../../../../../cauchy-stress-tensor.md) gives

$$
\frac{dE_{\rm bulk}}{dt}=\int_S w_t\cdot t_w\,dS,
\qquad t_w=\sigma(w)n.
$$

All interior terms cancel: the [strain](../../../../../strain.md) term is exactly the time derivative of elastic [energy](../../../../../energy.md).

For the restoring boundary law, $t_w=kw$. The prescribed support displacement cancels in the difference. Since $k$ is a time-independent [symmetric matrix](../../../../../symmetric-matrix.md),

$$
\int_Sw_t\cdot kw\,dS=\frac12\frac{d}{dt}\int_Sw\cdot kw\,dS.
$$

Hence the [elastic energy uniqueness with restoring boundary springs](../../../../../elastic-energy-uniqueness-with-restoring-boundary-springs.md) identity is

$$
\boxed{\frac{d}{dt}\left(E_{\rm bulk}-\frac12\int_Sw\cdot kw\,dS\right)=0.}
$$

The boundary contribution is nonnegative because $k$ is negative semidefinite. The initial difference and its [velocity](../../../../../velocity.md) vanish, so the conserved [energy](../../../../../energy.md) is zero. Its kinetic term implies $w_t=0$ everywhere; the zero initial displacement then gives $w=0$. This proves **uniqueness** without needing to exclude rigid displacements separately.

Physically, $-k$ is a nonnegative boundary spring-stiffness matrix, and the prescribed vector $U$ is the moving support position. The [traction](../../../../../traction.md) restores the displacement towards that support; null directions of $k$ have no spring force. The interpretation and conserved-energy proof use a fixed spring matrix, as indicated by the given boundary law.

On the mixed part $S_1$, write $t=\sigma n$. The condition is

$$
(I-nn^{\mathsf T})t=n\times F,\qquad u\cdot n=N.
$$

Thus the tangential [traction](../../../../../traction.md) and normal displacement are prescribed. The normal [traction](../../../../../traction.md) is a constraint reaction; tangential displacement is free. Only the tangential component of $F$ matters. On $S_2$, the entire displacement is prescribed.

For the difference of two such solutions, $w\cdot n=0$ and $(I-nn^{\mathsf T})t_w=0$ on $S_1$. Consequently $w_t$ is tangential and $t_w$ normal, so $w_t\cdot t_w=0$. On $S_2$, $w_t=0$. The boundary power vanishes everywhere, giving $dE_{\rm bulk}/dt=0$. The same zero-initial-energy argument gives $w=0$. Therefore **the mixed boundary problem also has at most one solution**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
