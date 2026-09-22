<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Minkowski spacetime](../../../../../minkowski-spacetime.md) with $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and units $\hbar=c=1$. The transformation rotates the two components in their internal plane. In particular,

$$
\delta(\phi_1^2+\phi_2^2)=2\alpha(\phi_1\phi_2-\phi_2\phi_1)=0,
\qquad
\delta\bigl(\partial_\mu\phi_1\partial^\mu\phi_1+\partial_\mu\phi_2\partial^\mu\phi_2\bigr)=0.
$$

Thus both terms in the [Lagrangian density](../../../../../lagrangian-density.md) are invariant: this is an [internal rotation symmetry of two real scalar fields](../../../../../internal-rotation-symmetry-of-two-real-scalar-fields.md), rather than a transformation of spacetime. The equal masses are essential to this symmetry.

The [Noether theorem](../../../../../noether-theorem.md) gives the [Noether current](../../../../../noether-current.md)

$$
j^\mu=\sum_{k=1}^2\frac{\partial\mathcal L}{\partial(\partial_\mu\phi_k)}\frac{\delta\phi_k}{\alpha}
=\phi_2\partial^\mu\phi_1-\phi_1\partial^\mu\phi_2.
$$

Indeed, the cross terms in its divergence cancel, and the two [Klein-Gordon equations](../../../../../klein-gordon-equation.md) imply

$$
\partial_\mu j^\mu=\phi_2\Box\phi_1-\phi_1\Box\phi_2
=-m^2\phi_2\phi_1+m^2\phi_1\phi_2=0.
$$

For fields decaying sufficiently at spatial infinity, there is no outward current flux. The conserved [Noether charge](../../../../../noether-charge.md) is therefore

$$
\boxed{Q=\int d^3x\,(\phi_2\dot\phi_1-\phi_1\dot\phi_2).}
$$

In [canonical quantization](../../../../../canonical-quantization.md), the [canonical momenta](../../../../../canonical-momentum.md) are $\pi_k=\dot\phi_k$, with equal-time [canonical commutation relations](../../../../../canonical-commutation-relation.md)

$$
[\phi_k(\mathbf x),\pi_l(\mathbf y)]=i\delta_{kl}\delta^3(\mathbf x-\mathbf y),
\qquad [\phi_k,\phi_l]=[\pi_k,\pi_l]=0.
$$

Consequently $Q=\int d^3x\,(\pi_1\phi_2-\pi_2\phi_1)$. Operators of different components commute, so this expression is [Hermitian](../../../../../hermitian-operator.md) without an ordering correction. Write $\int_{\mathbf p}=\int d^3p/(2\pi)^3$, $E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$ and $a_{k\mathbf p}=a^k_{\mathbf p}$. Substituting the oscillator expansions and using the [Dirac delta function](../../../../../dirac-delta-function.md) from the spatial integral gives

$$
Q=-\frac i2\int_{\mathbf p}\left[
(a_{1\mathbf p}-a_{1,-\mathbf p}^{\dagger})(a_{2,-\mathbf p}+a_{2\mathbf p}^{\dagger})
-(a_{2\mathbf p}-a_{2,-\mathbf p}^{\dagger})(a_{1,-\mathbf p}+a_{1\mathbf p}^{\dagger})
\right].
$$

The terms with two [annihilation operators](../../../../../annihilation-operator.md) cancel after $\mathbf p\mapsto-\mathbf p$; the terms with two [creation operators](../../../../../creation-operator.md) cancel in the same way. In the remaining terms use

$$
[a_{k\mathbf p},a_{l\mathbf q}^{\dagger}]=(2\pi)^3\delta_{kl}\delta^3(\mathbf p-\mathbf q).
$$

There is no [commutator](../../../../../commutator.md) constant between the distinct components. The result is already in [normal ordering](../../../../../normal-ordering.md):

$$
\boxed{Q=-i\int_{\mathbf p}\bigl(a_{2\mathbf p}^{\dagger}a_{1\mathbf p}-a_{1\mathbf p}^{\dagger}a_{2\mathbf p}\bigr).}
$$

For the [charged oscillator basis of a scalar doublet](../../../../../charged-oscillator-basis-of-a-scalar-doublet.md), compute

$$
[Q,a_{1\mathbf p}^{\dagger}]=-ia_{2\mathbf p}^{\dagger},\qquad
[Q,a_{2\mathbf p}^{\dagger}]=ia_{1\mathbf p}^{\dagger},\qquad
b_{\pm\mathbf p}^{\dagger}=\frac{a_{1\mathbf p}^{\dagger}\mp ia_{2\mathbf p}^{\dagger}}{\sqrt2}.
$$

It follows that $[Q,b_{\pm\mathbf p}^{\dagger}]=\pm b_{\pm\mathbf p}^{\dagger}$. The [Fock vacuum](../../../../../fock-vacuum.md) satisfies $Q|0\rangle=0$, so **$b_{+\mathbf p}^{\dagger}|0\rangle$ has charge $+1$, and $b_{-\mathbf p}^{\dagger}|0\rangle$ has charge $-1$**. To obtain a normalized [one-particle state](../../../../../one-particle-state.md), replace the sharp momentum by $\int_{\mathbf p}f(\mathbf p)b_{\pm\mathbf p}^{\dagger}|0\rangle$, where $\int_{\mathbf p}|f(\mathbf p)|^2=1$. The charge is unchanged. Equivalently,

$$
Q=\int_{\mathbf p}(b_{+\mathbf p}^{\dagger}b_{+\mathbf p}-b_{-\mathbf p}^{\dagger}b_{-\mathbf p}).
$$

The generator convention is $\delta\phi_k=i\alpha[Q,\phi_k]$, which reproduces the original rotation signs.

For [stability of a two-scalar quartic potential](../../../../../stability-of-a-two-scalar-quartic-potential.md), the relevant [potential energy](../../../../../potential-energy.md) density is

$$
V=\frac{m^2}{2}(\phi_1^2+\phi_2^2)+V_4,\qquad
V_4=\lambda(\phi_1^2-\phi_2^2)^2+2(\lambda+\mu)\phi_1^2\phi_2^2.
$$

Along either axis boundedness requires $\lambda\ge0$; along $\phi_1=\phi_2$ it requires $\lambda+\mu\ge0$. Conversely the displayed sum is nonnegative whenever both conditions hold. With $m^2>0$ the origin is then the unique global minimum, including the equality cases. Hence the stable-vacuum conditions are

$$
\boxed{\lambda\ge0,\qquad\mu\ge-\lambda.}
$$

Strict positivity of the quartic term away from the origin would instead require $\lambda>0$ and $\mu>-\lambda$. That stronger condition is unnecessary for a positive mass term. If $m=0$, the same non-strict conditions give boundedness, but the equality cases have flat directions and do not give an isolated [classical vacuum](../../../../../classical-vacuum.md).

Finally, the interaction changes the variation of the [potential energy](../../../../../potential-energy.md) by

$$
\delta V_4=4\alpha(\lambda-\mu)\phi_1\phi_2(\phi_1^2-\phi_2^2).
$$

The interacting [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) consequently give

$$
\partial_\mu j^\mu=-4(\lambda-\mu)\phi_1\phi_2(\phi_1^2-\phi_2^2).
$$

Thus the same [Noether charge](../../../../../noether-charge.md) is conserved for all field configurations precisely when **$\mu=\lambda$**. Then $V_4=\lambda(\phi_1^2+\phi_2^2)^2$ preserves the [internal rotation symmetry of two real scalar fields](../../../../../internal-rotation-symmetry-of-two-real-scalar-fields.md); imposing stability additionally requires $\lambda\ge0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
