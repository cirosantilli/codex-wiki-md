<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Fix the sign convention $\iota_{\xi_M}\omega=-d\mu^\xi$, where $\xi_M$ is the [fundamental vector field](../../../../../fundamental-vector-field.md) and $\mu^\xi=\langle\mu,\xi\rangle$. A [Hamiltonian group action](../../../../../hamiltonian-group-action.md) is a symplectic [Lie group action](../../../../../lie-group-action.md) together with an equivariant [moment map](../../../../../moment-map.md) $\mu:M\to\mathfrak g^*$ satisfying this identity for every $\xi\in\mathfrak g$. Equivariance means $\mu(gx)=\operatorname{Ad}_{g^{-1}}^*\mu(x)$. Merely requiring each fundamental field to have some Hamiltonian is the weaker condition of a [weakly Hamiltonian action](../../../../../weakly-hamiltonian-action.md).

For a [circle group](../../../../../circle-group.md) action, identify its Lie algebra with $\mathbb R$, and let $Y$ generate the action. Put $Z=\mu^{-1}(t)$ and let $i:Z\hookrightarrow M$. Since $t$ is a [regular value](../../../../../regular-value.md),

$$
T_xZ=\ker d\mu_x=\{v:\omega(Y_x,v)=0\}.
$$

The action is free, so $Y_x\ne0$. The [symplectic orthogonal complement](../../../../../symplectic-orthogonal-complement.md) of this hyperplane is exactly $\mathbb RY_x$, which is contained in $T_xZ$. Thus

$$
\ker(i^*\omega)_x=\mathbb RY_x.
$$

The free action of the compact [circle group](../../../../../circle-group.md) is proper, and the quotient $Q=Z/S^1$ is a [smooth manifold](../../../../../smooth-manifold.md) with projection $\pi:Z\to Q$ a [principal bundle](../../../../../principal-bundle.md). The form $i^*\omega$ is invariant and kills the orbit directions, hence is basic and descends to a unique two-form $\omega_Q$ satisfying $\pi^*\omega_Q=i^*\omega$. It is closed because pullback by a [submersion](../../../../../submersion.md) detects [differential forms](../../../../../differential-form-split.md). If a quotient tangent vector annihilates $\omega_Q$, a lift lies in the displayed [kernel](../../../../../kernel-of-a-linear-map.md) and hence projects to zero. Therefore $\omega_Q$ is nondegenerate. This proves [symplectic reduction](../../../../../symplectic-reduction.md) directly.

If $L\subset Q$ is a [Lagrangian submanifold](../../../../../lagrangian-submanifold.md), its inverse image $\widetilde L=\pi^{-1}(L)$ is a smooth [circle bundle](../../../../../circle-bundle.md) over $L$. The restricted [symplectic form](../../../../../symplectic-form.md) is $\pi^*(\omega_Q|_L)=0$. If $\dim M=2N$, then $\dim Q=2N-2$, $\dim L=N-1$, and $\dim\widetilde L=N$, proving that $\widetilde L$ is Lagrangian. This is the [Lagrangian lift through circle reduction](../../../../../lagrangian-lift-through-circle-reduction.md).

For scalar multiplication on $\mathbb C^{n+1}$, the generator is $Y=\sum_j(-y_j\partial_{x_j}+x_j\partial_{y_j})$. Direct contraction gives

$$
\iota_Y\omega_{st}=-\sum_j(x_jdx_j+y_jdy_j),\qquad\boxed{\mu(z)=\tfrac12|z|^2.}
$$

Choose $t>0$. Its level is the sphere of radius $R=\sqrt{2t}$ and its quotient is $\mathbb{CP}^n$. [Complex conjugation](../../../../../complex-conjugation.md) on the sphere reverses the ambient [symplectic form](../../../../../symplectic-form.md) and descends to an [anti-symplectic involution](../../../../../anti-symplectic-involution.md) of the quotient. Its fixed set is $\mathbb{RP}^n$: a projective point fixed by conjugation has a real representative after a phase change. For two tangent vectors to this fixed set, anti-symplecticity makes the reduced form equal to its negative, so it vanishes. The real dimension is $n$, half the quotient dimension, proving the [Lagrangian fixed locus of an anti-symplectic involution](../../../../../lagrangian-fixed-locus-of-an-anti-symplectic-involution.md) property.

The lifted [Lagrangian submanifold](../../../../../lagrangian-submanifold.md) can be written explicitly as

$$
\boxed{\widetilde L=\{e^{i\theta}x:x\in\mathbb R^{n+1},\ |x|=R\}
\cong(S^n\times S^1)/((x,\zeta)\sim(-x,-\zeta)).}
$$

The only redundancy in this parametrization is the displayed free involution: two nonzero real representatives on the same complex ray differ by a real sign. The quotient embeds smoothly in the sphere, and projection to $[x]\in\mathbb{RP}^n$ exhibits its [circle bundle](../../../../../circle-bundle.md) structure. Its Lagrangian property follows from the reduction argument, including the case $n=0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
