<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $d\ge2$, let $\omega$ be a [Conformal Killing vector field](../../../../../conformal-killing-vector-field.md), put $\sigma=\partial\cdot\omega/d$, and assign the massless [scalar field](../../../../../scalar-field.md) [scaling dimension](../../../../../scaling-dimension.md) $\Delta=(d-2)/2$. In a finite [conformal transformation](../../../../../conformal-map.md) with metric scale $\Omega^2$, the transformation law is $\phi'(x')=\Omega(x)^{-\Delta}\phi(x)$. Its infinitesimal fixed-coordinate form is

$$
\delta_0\phi=-\omega^\mu\partial_\mu\phi-\Delta\sigma\phi.
$$

For $\mathcal L=(\partial\phi)^2/2$, contract the [Conformal Killing equation](../../../../../conformal-killing-equation.md) with $\partial_\mu\phi\partial_\nu\phi$. Direct differentiation then gives

$$
\begin{aligned}
\delta_0\mathcal L
&=-\omega\cdot\partial\mathcal L-(1+\Delta)\sigma(\partial\phi)^2-\frac\Delta2\partial_\mu(\phi^2)\partial^\mu\sigma\\
&=-\partial_\mu(\omega^\mu\mathcal L)-\frac\Delta2\partial_\mu(\phi^2\partial^\mu\sigma)+\frac\Delta2\phi^2\Box\sigma.
\end{aligned}
$$

Here $2(1+\Delta)=d$. [Flat conformal Killing integrability](../../../../../flat-conformal-killing-integrability.md) gives $\Box\sigma=0$, with the Lorentzian version obtained by replacing the flat metric consistently. Thus the action variation is a boundary integral, vanishing for suitable [boundary conditions](../../../../../boundary-condition.md). This proves **conformal invariance with field dimension $(d-2)/2$**, without using the field equation. The connected finite symmetry follows by integrating the infinitesimal generators. Equivalently its [conformal currents](../../../../../conformal-current.md) follow from the [improved stress-energy tensor of a free massless scalar](../../../../../improved-stress-energy-tensor-of-a-free-massless-scalar.md).

In one dimension the metric conformality condition is vacuous. The same action-variation calculation contains $-\phi^2\omega'''/4$, so the free action is invariant under the projective subgroup $\omega'''=0$, rather than arbitrary reparametrizations. The usual field-theory conformal-invariance claim above concerns $d\ge2$.

In $d=2$, $\Delta=0$, so the field transforms simply as a scalar. There is no improvement term and no derivative of the conformal scale in the variation. All local independent reparametrizations of the two null coordinates preserve the action; after Euclidean continuation they are holomorphic and antiholomorphic maps. The conformal algebra is therefore infinite-dimensional, in contrast to $d>2$.

Now use Lorentzian coordinates with spatial period $\ell$. The [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\dot\phi$, and [canonical quantization](../../../../../canonical-quantization.md) imposes $[\phi(t,x),\pi(t,y)]=i\delta_\ell(x-y)$, with the periodic delta distribution $\delta_\ell(s)=\ell^{-1}\sum_{n\in\mathbb Z}e^{2\pi ins/\ell}$. Solving the wave equation and imposing reality gives a convenient oscillator normalization:

$$
\phi(t,x)=q+\frac{pt}{\ell}+\frac{i}{\sqrt{4\pi}}\sum_{n\ne0}\frac1n\left[\alpha_ne^{-2\pi in(t-x)/\ell}+\widetilde\alpha_ne^{-2\pi in(t+x)/\ell}\right].
$$

Strict spatial periodicity excludes a winding term. The [canonical commutation relation](../../../../../canonical-commutation-relation.md) is equivalent to

$$
[q,p]=i,\qquad [\alpha_m,\alpha_n]=m\delta_{m+n,0},\qquad
[\widetilde\alpha_m,\widetilde\alpha_n]=m\delta_{m+n,0},\qquad [\alpha_m,\widetilde\alpha_n]=0,
$$

with $\alpha_n^\dagger=\alpha_{-n}$ and the corresponding tilded relation. Both oscillator families commute with $q,p$. To verify the normalization, the zero-mode commutator supplies $i/\ell$, while each oscillator family supplies $i(2\ell)^{-1}\sum_{n\ne0}e^{2\pi in(x-y)/\ell}$. Their sum is exactly $i\delta_\ell(x-y)$. The positive-index modes are [annihilation operators](../../../../../annihilation-operator.md) and the negative-index modes are [creation operators](../../../../../creation-operator.md), giving two independent [bosonic Fock spaces](../../../../../bosonic-fock-space.md) together with the free-particle zero mode.

Define $\alpha_0=\widetilde\alpha_0=p/\sqrt{4\pi}$ and the [normal ordering](../../../../../normal-ordering.md) quadratic generators

$$
L_m=\frac12\sum_{n\in\mathbb Z}:\alpha_{m-n}\alpha_n:,
\qquad \widetilde L_m=\frac12\sum_{n\in\mathbb Z}:\widetilde\alpha_{m-n}\widetilde\alpha_n:.
$$

These are the Fourier modes of the two chiral components of the [stress-energy tensor](../../../../../stress-energy-tensor.md). The oscillator [operator commutators](../../../../../operator-commutator.md) immediately give $[L_m,\alpha_n]=-n\alpha_{m+n}$. Applying this to both factors of $L_n$ gives $(m-n)L_{m+n}$, except for a scalar term when $m+n=0$, produced by reordering creators and annihilators. Its value is independent of the momentum sector. Evaluate it in the formal zero-momentum oscillator vacuum. For $m>0$,

$$
L_{-m}|0\rangle=\frac12\sum_{r=1}^{m-1}\alpha_{-r}\alpha_{-(m-r)}|0\rangle,
\qquad
\langle0|L_mL_{-m}|0\rangle=\frac12\sum_{r=1}^{m-1}r(m-r)=\frac{m^3-m}{12}.
$$

The two contractions of each pair explain the factor $1/2$. Hence the [free-boson Virasoro central term](../../../../../free-boson-virasoro-central-term.md) yields

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}+\frac{m^3-m}{12}\delta_{m+n,0}},\qquad \boxed{c=1}.
$$

The tilded modes give a second commuting [Virasoro algebra](../../../../../virasoro-algebra.md) with $\bar c=1$. The adjoint condition $L_m^\dagger=L_{-m}$ and the positive oscillator norms make this a [unitary highest-weight Virasoro representation](../../../../../unitary-highest-weight-virasoro-module.md) in each momentum sector. In a fixed momentum sector, $L_0=p^2/(8\pi)+\sum_{n>0}\alpha_{-n}\alpha_n$, so the oscillator ground state is a highest-weight state of weight $p^2/(8\pi)$ in either sector. For a noncompact field the zero mode is a free particle: definite momentum ground states are generalized states, rather than a normalizable zero-mode vacuum. The oscillator representation and central term remain well defined. With the standard cylinder vacuum-energy subtraction, the Hamiltonian is

$$
\boxed{H=\frac{2\pi}{\ell}\left(L_0+\widetilde L_0-\frac1{12}\right)}.
$$

The constant is the [Casimir energy of a two-dimensional conformal field theory](../../../../../casimir-energy-of-a-two-dimensional-conformal-field-theory.md); omitting it amounts to a different additive Hamiltonian convention, not a change of the plane [Virasoro algebra](../../../../../virasoro-algebra.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
