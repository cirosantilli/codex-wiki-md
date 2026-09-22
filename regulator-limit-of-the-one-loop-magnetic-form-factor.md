# Regulator limit of the one-loop magnetic form factor

↑ **Parent:** [Schwinger correction to the electron magnetic moment](schwinger-correction-to-the-electron-magnetic-moment.md)

In [Feynman gauge](feynman-gauge.md), use the auxiliary [photon propagator](photon-propagator.md) $-ig_{\mu\nu}/(k^2-\lambda^2+i0)$ and $r=\lambda/m>0$. The projected one-loop [Feynman parameter](feynman-parameter.md) integral is

$$
F_2^{(1)}(0;\lambda)=\frac{\alpha}{2\pi}I(r),
\qquad
I(r)=\int_0^1\frac{2x(1-x)^2}{(1-x)^2+xr^2}\,dx.
$$

Here $x$ is the source's photon parameter $z$.[Eqs. (32), (35), (40), (68)](qed-vertex-correction-vadim-kaplunovsky-course-notes.md)

To check the reduction, use $N_2=4z(1-z)m^2$ and $\Delta'=(1-z)^2m^2+z\lambda^2$. The three-parameter expression has prefactor $e^2/(16\pi^2)$ multiplying $N_2/\Delta'$. At fixed $z$, $\int_0^{1-z}du=1-z$, giving $e^2/(4\pi^2)\int_0^1 z(1-z)^2/[(1-z)^2+zr^2]\,dz$. Substituting $e^2=4\pi\alpha$ gives exactly the displayed integral. This starts from the projected [QED](quantum-electrodynamics.md) numerator; it is not a derivation of the whole [QED](quantum-electrodynamics.md) calculation from an arbitrarily chosen integral.

The regulator can then be removed by a short independent argument. Write its integrand as $f_r(x)$. For $0\le x<1$, $f_r(x)\to2x$, and

$$
0\le f_r(x)=2x\frac{(1-x)^2}{(1-x)^2+xr^2}\le2x,
\qquad\int_0^1 2x\,dx=1.
$$

The [dominated convergence theorem](dominated-convergence-theorem.md) therefore gives $I(r)\to1$ and $F_2^{(1)}(0)=\alpha/(2\pi)$. At $x=1$ the regulated integrand is zero, whereas the limiting function can be assigned value $2$; one point has zero measure and changes no integral. For every $r>0$, $0<I(r)<1$, and decreasing $r$ increases the integral. The visible suppression near $x=1$ narrows as the regulator shrinks; it is not a uniform pointwise approximation at that endpoint.

<a id="image-a-finite-magnetic-coefficient-survives-removal-of-the-regulator"></a>
![](qed-magnetic-anomaly-regulator-limit.png)

**[Figure 6](#image-a-finite-magnetic-coefficient-survives-removal-of-the-regulator). A finite magnetic coefficient survives removal of the regulator**. Original numerical evaluation of the reduced one-loop [Feynman parameter](feynman-parameter.md) integral, with $r=\lambda/m$. The left panel shows suppression near the endpoint; the right panel plots $I(r)=F_2^{(1)}(0;\lambda)/(\alpha/2\pi)$ against the auxiliary mass ratio. The dashed limit is the exact integral $\int_0^1 2x\,dx=1$. Finite $r$ values illustrate [regularization in quantum field theory](regularization-in-quantum-field-theory.md), not alternative measured [photon](photon.md) masses.

This auxiliary mass regulates an [infrared divergence](infrared-divergence.md), not an [ultraviolet divergence](ultraviolet-divergence.md); the finite-mass prescription alone is not fully [gauge-invariant](gauge-invariance.md).[p. 15, Eqs. (65)–(68)](qed-vertex-correction-vadim-kaplunovsky-course-notes.md)

The ultraviolet problem belongs to the full [QED](quantum-electrodynamics.md) amplitude. [Electron self-energy](electron-self-energy.md), [wave-function renormalization](wave-function-renormalization.md) and the charge vertex require consistent [counterterms](counterterm.md) and [renormalization conditions](renormalization-condition.md). The [Ward identity for QED renormalization constants](ward-identity-for-qed-renormalization-constants.md) ties $Z_1$ to $Z_2$, rather than allowing the vertex and external [electron](electron.md) normalization to be fitted independently. Minimal renormalizable [QED](quantum-electrodynamics.md) has no independent [Pauli term](pauli-term.md) to adjust this finite one-loop $F_2(0)$: its dimension-five coefficient is predicted from the [mass](mass.md) and [electric charge](electric-charge-split.md) inputs. Adding a free [Pauli term](pauli-term.md) would define a different theory with an extra parameter. Finiteness of the reduced integral alone proves neither all-order [renormalizability](renormalizable-quantum-field-theory.md) nor finiteness of every [QED](quantum-electrodynamics.md) observable.

## ↑ Ancestors (7)

1. [Schwinger correction to the electron magnetic moment](schwinger-correction-to-the-electron-magnetic-moment.md)
2. [Quantum electrodynamics](quantum-electrodynamics.md)
3. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
4. [Quantum field theory](quantum-field-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
