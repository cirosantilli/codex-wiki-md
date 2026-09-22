<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an auxiliary field varying slowly over lattice distances, measure $x$ in lattice-spacing units and replace the squared difference by $(dm/dx)^2$. The long-wavelength action becomes

$$
S_E[m]=\int_0^Ldx\left[\frac{M_Q}2\left(\frac{dm}{dx}\right)^2+U(m)\right],\qquad
M_Q=\frac1{J\sinh\kappa}.
$$

This is the [Euclidean path integral](../../../../../../euclidean-path-integral.md) of a one-coordinate quantum particle, with the classical spatial coordinate serving as imaginary time and $\hbar=1$. To see the correspondence at the operator level, time-slice it by $\epsilon$ and use the symmetric kernel

$$
K_\epsilon(m',m)=\left(\frac{M_Q}{2\pi\epsilon}\right)^{1/2}
\exp\left[-\frac{M_Q(m'-m)^2}{2\epsilon}-\frac\epsilon2\{U(m')+U(m)\}\right].
$$

Acting on a smooth test function, Gaussian integration gives $K_\epsilon\psi=\psi+\epsilon\psi''/(2M_Q)-\epsilon U\psi+O(\epsilon^2)$. Thus the continuum [auxiliary-field transfer operator for an Ising chain](../../../../../../auxiliary-field-transfer-operator-for-an-ising-chain.md) is $e^{-\epsilon\widehat H_Q}$, where

$$
\boxed{\widehat H_Q=-\frac1{2M_Q}\frac{d^2}{dm^2}+U(m)
=-\frac{J\sinh\kappa}{2}\frac{d^2}{dm^2}+U(m).}
$$

Multiplying kernels and integrating over intermediate fields gives $\langle m_f|e^{-L\widehat H_Q}|m_i\rangle$ for fixed endpoints, and $\operatorname{tr}e^{-L\widehat H_Q}$ for periodic fields, up to the normalization already absorbed in $C$. This is the precise [classical Ising chain as a quantum particle](../../../../../../classical-ising-chain-as-a-quantum-particle.md) correspondence. It concerns an imaginary-time transition kernel; it is not the squared modulus of a real-time transition amplitude. The continuum approximation retains smooth long-distance modes, rather than asserting exact equality of the finite-spacing transfer operator with this differential operator.

At $h=0$, set $A=\tanh(\kappa/2)/J$. Expansion of the local potential gives

$$
U(m)=-\log2+(A-2)m^2+\frac43m^4+O(m^6),\qquad
U'(m)=2Am-2\tanh(2m).
$$

The potential is even and grows as $Am^2-2|m|$ at large $|m|$. It is a symmetric double well precisely when

$$
\boxed{A<2,\qquad J>\tfrac12\tanh(\kappa/2).}
$$

The nonzero stationary points satisfy $Am=\tanh(2m)$. For $m>0$, the ratio $\tanh(2m)/m$ decreases strictly from 2 to 0: writing $z=2m$, the sign follows from $\tanh z-z\operatorname{sech}^2z>0$, whose derivative is $2z\operatorname{sech}^2z\tanh z>0$. Hence there is one minimum on each side when $A<2$. At $A=2$ the potential instead has a single quartic minimum, and for $A>2$ a single quadratic minimum. Small $\kappa$ with fixed positive $J$ falls in the double-well regime, but the printed claim requires this coupling condition; $\kappa\ll1$ alone does not imply it if $J$ scales to zero too quickly.

A weak magnetic field gives

$$
U(m,h)=U(m,0)-h\tanh(2m)+O(h^2),\qquad U(-m,h)=U(m,-h).
$$

The linear term is odd in $m$. For positive $h$, the positive well becomes deeper. If the zero-field minima are $\pm m_*$, their depth difference to first order is $U(m_*,h)-U(-m_*,h)=-2h\tanh(2m_*)$. **The magnetic field tilts the symmetric double well and favors the matching spin orientation.** A large enough field can eliminate the metastable well.

Finally, two minima do not imply a true finite-temperature [phase transition](../../../../../../phase-transition.md) in this one-dimensional chain at fixed finite interaction range $1/\kappa$. A finite quantum barrier permits [quantum tunnelling](../../../../../../quantum-tunnelling.md); the confining one-dimensional [Schrödinger operator](../../../../../../schrodinger-operator.md) has a unique symmetric [ground state](../../../../../../ground-state.md) at zero field and a nonzero first excitation gap. The quantum gap corresponds to a finite classical [correlation length](../../../../../../correlation-length.md). A very small gap can mimic ordering on a finite sample, but genuine degeneracy requires a singular limit such as vanishing tunnelling. This distinction is central to interpreting the quantum mapping.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
