<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\Omega$ be the solid exterior to the cavity, and choose $\mathbf n$ outward from the solid, hence into the cavity on its boundary $S$. Subtraction of the incident solution from the total solution gives the scattered [displacement field](../../../../../displacement-field-mechanics.md) equations

$$
\rho\ddot u_i^s=\partial_j\sigma_{ij}^s,\qquad
\sigma_{ij}^s=c_{ijkl}e_{kl}^s,\qquad
e_{kl}^s=\tfrac12(u_{k,l}^s+u_{l,k}^s),\qquad \mathbf x\in\Omega.
$$

The traction-free cavity condition for the total field gives **$\sigma_{ij}^s n_j=-\sigma_{ij}^0 n_j$ on $S$**. The scattered field has zero [initial displacement](../../../../../initial-displacement.md) and [initial velocity](../../../../../initial-velocity.md) before the pulse reaches the cavity and satisfies an outgoing [radiation condition](../../../../../radiation-condition.md), excluding an additional incoming [elastic wave](../../../../../elastic-wave.md). Equivalently one seeks the causal response to this prescribed boundary [traction](../../../../../traction.md). Although the incident plane pulse extends across an infinite plane, the causal scattered field from the bounded cavity has finite propagation distance at each finite time.

To prove [energy uniqueness for traction-driven elasticity](../../../../../energy-uniqueness-for-traction-driven-elasticity.md), take the difference $\mathbf w$ of two solutions with the same [initial conditions](../../../../../initial-condition.md), [body force](../../../../../body-force.md), boundary [traction](../../../../../traction.md) and outgoing condition. It satisfies

$$
\rho\ddot w_i=\partial_j\sigma_{ij}(w),\quad
\sigma_{ij}(w)n_j=0\text{ on }S,\quad
\mathbf w(\cdot,t_0)=\dot{\mathbf w}(\cdot,t_0)=0.
$$

For a large enclosing ball $B_L$, multiply by $\dot w_i$ and integrate over $\Omega\cap B_L$. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_{\Omega\cap B_L}\rho\ddot w_i\dot w_i\,dV
=\int_{\partial(\Omega\cap B_L)}\dot w_i\sigma_{ij}(w)n_j\,dS
-\int_{\Omega\cap B_L}\sigma_{ij}(w)\partial_j\dot w_i\,dV.
$$

Symmetry of [stress](../../../../../stress.md) replaces the last derivative by $\dot e_{ij}(w)$, and major symmetry of the [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md) makes that integral the derivative of the [strain](../../../../../strain.md) [energy](../../../../../energy.md). Therefore

$$
\frac{d}{dt}\frac12\int_{\Omega\cap B_L}
[\rho|\dot{\mathbf w}|^2+c_{ijkl}e_{ij}(w)e_{kl}(w)]\,dV
=\int_{\partial(\Omega\cap B_L)}\dot w_i\sigma_{ij}(w)n_j\,dS.
$$

The cavity contribution is zero. On any fixed finite time interval choose $L$ beyond the causal support of the scattered difference; the outer contribution is then zero as well. This gives conservation of its nonnegative [elastic energy](../../../../../elastic-energy.md). Positive [mass density](../../../../../density.md) and positive [strain](../../../../../strain.md) [energy](../../../../../energy.md) imply that zero initial [energy](../../../../../energy.md) forces $\dot{\mathbf w}=0$ everywhere; the zero initial [displacement field](../../../../../displacement-field-mechanics.md) then gives $\mathbf w=0$. The same argument works for finite-energy outgoing solutions by taking the limit of enclosing surfaces and excluding incoming [energy](../../../../../energy.md). Hence **the causal scattered field $\mathbf u^s$ is unique**. Specifying the incident field and cavity [traction](../../../../../traction.md) alone without the initial and outgoing conditions would not establish uniqueness.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
