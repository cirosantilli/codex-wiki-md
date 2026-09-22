<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite-dimensional mechanical system let $Q$ be its [configuration space](../../../../../mechanical-configuration-space.md), a smooth manifold incorporating the holonomic constraints. [Lagrangian mechanics](../../../../../lagrangian-mechanics.md) starts with $L:TQ\to\mathbb R$; a curve $q(t)$ makes the action stationary under fixed-endpoint variations. The resulting equations are

$$
\frac{d}{dt}\frac{\partial L}{\partial v^i}-\frac{\partial L}{\partial q^i}=0.
$$

This equation is coordinate-independent even though generalized coordinates give its familiar expression.

The fibre derivative $\mathbb FL(q,v)=(q,p)$, with $p_i=L_{v^i}$, defines the [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md). The [Cartan form of a regular mechanical Lagrangian](../../../../../cartan-form-of-a-regular-mechanical-lagrangian.md) is

$$
\theta_L=p_i\,dq^i,\qquad\omega_L=-d\theta_L,\qquad E_L=p_iv^i-L.
$$

For a [regular Lagrangian](../../../../../regular-lagrangian.md), the velocity Hessian is invertible, $\omega_L$ is symplectic, and $\iota_{\Gamma_L}\omega_L=dE_L$ determines a second-order vector field on $TQ$. In coordinates this recovers the displayed Euler–Lagrange equations: the velocity components of the vector field are $v^i$, and its acceleration components are fixed by the invertible Hessian.

[Hamiltonian mechanics](../../../../../hamiltonian-mechanics.md) takes place on $T^*Q$. Its [tautological one-form](../../../../../canonical-one-form-on-a-cotangent-bundle.md) is $\theta=p_i\,dq^i$, and its canonical [symplectic form](../../../../../symplectic-form.md) is $\omega=-d\theta=dq^i\wedge dp_i$. With $\iota_{X_H}\omega=dH$,

$$
\boxed{\dot q^i=H_{p_i},\qquad\dot p_i=-H_{q^i}.}
$$

The associated [Poisson bracket](../../../../../poisson-bracket.md) is $\{f,g\}=f_{q^i}g_{p_i}-f_{p_i}g_{q^i}$, so $X_Hf=\{f,H\}$. For a [hyperregular Lagrangian](../../../../../hyperregular-lagrangian.md), $\mathbb FL$ is a global diffeomorphism, $H=E_L\circ(\mathbb FL)^{-1}$ and $(\mathbb FL)^*\omega=\omega_L$. The two formulations then describe the same trajectories. Regularity gives only local equivalence; degenerate Lagrangians require constraint analysis instead. These geometric structures distinguish equations of motion from arbitrary coordinate formulae and make [symmetry](../../../../../symmetry-physics.md) reduction precise.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
