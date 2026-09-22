<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the [exact differential form](../../../../../../exact-differential-form.md) as $\alpha=du$ for a smooth real-valued function $u$ on $N$. On $T^*N$ take the [Hamiltonian function](../../../../../../hamiltonian-function.md) $H=u\circ\pi$. With $\omega=\sum_jdq_j\wedge dp_j$ and $\iota_{X_H}\omega=-dH$, the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) is

$$
X_H=\sum_j\frac{\partial u}{\partial q_j}\frac{\partial}{\partial p_j}.
$$

Its complete flow is explicit:

$$
\boxed{\phi_H^t(q,p)=(q,p+t\,du_q)}.
$$

The base point stays fixed, so this flow exists for all real $t$, even if $u$ is unbounded on a noncompact base. Its time-one map is exactly $f$, proving that the [cotangent fiber translation](../../../../../../cotangent-fiber-translation.md) is a [Hamiltonian diffeomorphism](../../../../../../hamiltonian-isotopy.md) in the unrestricted complete-flow group.

This construction also justifies the hint for this family, without treating exactness as a general substitute for a Hamiltonian isotopy. For any [Hamiltonian isotopy](../../../../../../hamiltonian-isotopy.md) $\psi_t$ on this cotangent bundle, [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md), $d\theta=-\omega$ and $\iota_{X_{H_t}}\omega=-dH_t$ give

$$
\frac d{dt}\psi_t^*\theta=\psi_t^*\bigl(d(\theta(X_{H_t}))+\iota_{X_{H_t}}d\theta\bigr)=d\bigl(\psi_t^*(\theta(X_{H_t})+H_t)\bigr).
$$

Integrating proves that $\psi_1^*\theta-\theta$ is exact. For the present translation this difference is $\pi^*\alpha$, which is exact if and only if $\alpha$ is exact: one direction is pullback of $du$, and the other is pullback by the zero section. Necessity therefore follows from the differential identity, while sufficiency follows from the complete flow just constructed.

Compact support is a separate issue. If $du$ is nonzero at some $q$, the map moves every point of the entire unbounded fiber over $q$, so it is not a member of the [compactly supported Hamiltonian diffeomorphism group](../../../../../../compactly-supported-hamiltonian-diffeomorphism-group.md). For example $N=\mathbb R$, $u(q)=q$ gives $(q,p)\mapsto(q,p+1)$. Thus the claim about this global translation uses the full Hamiltonian group, not $\operatorname{Ham}_c$; its flow can be cut off to agree on a prescribed compact swept set, but such a cutoff does not give the same map on the entire cotangent bundle.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
