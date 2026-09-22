<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [Lagrangian submanifold](../../../../../lagrangian-submanifold.md) of a $2n$-dimensional [symplectic manifold](../../../../../symplectic-manifold.md) $(M,\omega)$ is an $n$-dimensional submanifold $L$ such that the pullback of $\omega$ to $L$ is zero. Equivalently, each tangent space $T_xL$ is its own symplectic orthogonal. The dimension condition makes it maximally isotropic: in a nondegenerate alternating vector space no isotropic subspace has dimension greater than $n$.

In [geometric quantization](../../../../../geometric-quantization.md), a line bundle with a [connection on a vector bundle](../../../../../connection-vector-bundle.md) whose curvature is proportional to $\omega/\hbar$ provides the initial quantum-state space. A real polarization foliates phase space locally by Lagrangian leaves; requiring sections to be covariantly constant along these leaves reduces their independent variables by half. The curvature restricts to zero on a Lagrangian leaf, allowing local flat sections. Globally its holonomy can impose the familiar [Bohr-Sommerfeld quantization](../../../../../bohr-sommerfeld-quantization.md) condition. Thus Lagrangian submanifolds describe choices of quantum configuration data and the support of semiclassical states, rather than requiring simultaneous sharp values of all position and momentum coordinates.

For the thermodynamic application, regard $(S,V,N)$ as base coordinates $q^i$ and $(T,-P,\mu)$ as fiber coordinates $p_i$ on $T^*\mathbb R^3$. The [canonical one-form on a cotangent bundle](../../../../../canonical-one-form-on-a-cotangent-bundle.md) and the position-first [symplectic form](../../../../../symplectic-form.md) are

$$
\theta=p_i\,dq^i=T\,dS-P\,dV+\mu\,dN,\qquad
\omega=-d\theta=dS\wedge dT-dV\wedge dP+dN\wedge d\mu.
$$

The negative sign in the pressure coordinate is essential. A smooth potential $M(S,V,N)$ determines the embedding

$$
\iota_M(S,V,N)=\bigl(S,V,N,M_S,M_V,M_N\bigr),
$$

where the last three coordinates are ordered as $(T,-P,\mu)$: explicitly $T=M_S$, $P=-M_V$, and $\mu=M_N$, so the second fiber coordinate is $-P=M_V$. Accordingly, in the actual $p_i$ coordinates the graph is

$$
\boxed{L_M=\{(S,V,N;p_S,p_V,p_N):
(p_S,p_V,p_N)=(M_S,M_V,M_N)\}.}
$$

Projection to the base is the identity, so this is an embedded three-dimensional submanifold, even if the Hessian of $M$ is degenerate. The [first law of thermodynamics](../../../../../first-law-of-thermodynamics.md) gives $\iota_M^*\theta=dM$. Hence

$$
\boxed{\iota_M^*\omega=-d(\iota_M^*\theta)=-d^2M=0.}
$$

It has half the dimension of the ambient cotangent bundle and is therefore Lagrangian. This proves the [thermodynamic potential as a Lagrangian graph](../../../../../thermodynamic-potential-as-a-lagrangian-graph.md) construction for every smooth choice of $M$, locally on any domain on which the potential is defined. No invertibility, extensivity or stability assumption is needed for this geometric conclusion.

In components the same vanishing follows from equality of mixed derivatives. The thermodynamic conjugate variables satisfy

$$
T_V=-P_S,\qquad T_N=\mu_S,\qquad -P_N=\mu_V.
$$

These cancel the three coefficients of the pulled-back two-form. They are the integrability relations behind the local thermodynamic potential, and demonstrate directly why the first-law graph is Lagrangian.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
