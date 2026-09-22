<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take the [Minkowski metric](../../../../../minkowski-metric.md) with signature $(+---)$ and a coupling $e\ne0$. For a [charged scalar field](../../../../../charged-scalar-field.md) use the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md)

$$
D_\mu\phi=(\partial_\mu-iea_\mu)\phi,
\qquad \phi'=e^{i\alpha}\phi,
\qquad a'_\mu=a_\mu+e^{-1}\partial_\mu\alpha.
$$

A [scalar electrodynamics](../../../../../scalar-electrodynamics.md) Lagrangian is

$$
\boxed{\mathcal L=-\frac14f_{\mu\nu}f^{\mu\nu}
+(D_\mu\phi)^*D^\mu\phi-V(|\phi|^2).}
$$

Any real potential bounded below and depending only on the modulus gives [gauge invariance](../../../../../gauge-invariance.md). Indeed,

$$
D'_\mu\phi'=e^{i\alpha}D_\mu\phi,
\qquad f'_{\mu\nu}=f_{\mu\nu},\qquad |\phi'|^2=|\phi|^2.
$$

The derivative of the phase cancels the shifted [gauge field](../../../../../gauge-field.md) in the first identity; commuting partial derivatives proves the second. These identities verify invariance of every term, including the interaction hidden in the kinetic term.

For an unbroken example choose $V=m_\phi^2|\phi|^2+\lambda|\phi|^4$ with $m_\phi^2>0$ and $\lambda>0$. The minimum is at zero. There is no vector [mass](../../../../../mass.md) term in the quadratic expansion and no [Higgs mechanism](../../../../../higgs-mechanism.md). Pure electromagnetic theory has a neutral massless [spin](../../../../../spin.md)-one [photon](../../../../../photon.md) with two physical transverse polarizations, equivalently helicities $+1$ and $-1$; longitudinal and time-component polarizations are gauge redundancies. In the unbroken scalar theory, the same massless [photon](../../../../../photon.md) is accompanied by a [spin](../../../../../spin.md)-zero charged particle and its oppositely charged [antiparticle](../../../../../antiparticle.md), both of [mass](../../../../../mass.md) $m_\phi$. A complex scalar has two real physical [degrees of freedom](../../../../../degree-of-freedom.md), rather than two unrelated charged species.

For a Higgs example choose

$$
V=\lambda\left(|\phi|^2-\frac{v^2}{2}\right)^2,\qquad \lambda>0,\quad v>0.
$$

The vacuum modulus is nonzero. Around one vacuum representative, [unitary gauge](../../../../../unitary-gauge.md) removes the phase and writes $\phi=(v+h)/\sqrt2$. Then

$$
(D_\mu\phi)^*D^\mu\phi
=\frac12\partial_\mu h\partial^\mu h+\frac12e^2(v+h)^2a_\mu a^\mu,
\qquad V=\lambda\left(vh+\frac{h^2}{2}\right)^2.
$$

Thus the quadratic spectrum is

$$
\boxed{m_A^2=e^2v^2,\qquad m_h^2=2\lambda v^2.}
$$

The [gauge boson](../../../../../gauge-boson.md) is a massive [spin](../../../../../spin.md)-one particle with three polarizations, and $h$ is a neutral massive [spin](../../../../../spin.md)-zero [Higgs boson](../../../../../higgs-boson.md). The scalar phase supplies the longitudinal vector polarization; it is not an extra physical massless [Goldstone boson](../../../../../goldstone-boson.md). The degree count is unchanged: two massless-vector polarizations plus two scalar degrees become three massive-vector polarizations plus one radial scalar degree. The underlying [gauge invariance](../../../../../gauge-invariance.md) remains a redundancy of the description.

For the two-charge theory, use

$$
D_\mu\phi=(\partial_\mu-iea_\mu)\phi,
\qquad D_\mu\psi=(\partial_\mu-2iea_\mu)\psi,
$$

and retain the same [gauge transformation](../../../../../gauge-transformation.md) of $a_\mu$. Both derivatives transform with the phase of their own field. A manifestly stable [two-charge scalar gauge potential](../../../../../two-charge-scalar-gauge-potential.md) is, for positive $m_\phi^2,M^2,\lambda_\phi,\lambda_\psi$, $g\ge0$ and a nonzero complex constant $b$,

$$
V(\phi,\psi)=m_\phi^2|\phi|^2+M^2|\psi-b\phi^2|^2
+\lambda_\phi|\phi|^4+\lambda_\psi|\psi|^4+g|\phi|^2|\psi|^2.
$$

Since $\psi-b\phi^2$ has charge $2e$, its modulus is [gauge-invariant](../../../../../gauge-invariance.md). Expanding its square exhibits the direct coupling

$$
-M^2\bigl(b\psi^*\phi^2+b^*\psi\phi^{*2}\bigr)
+M^2|b|^2|\phi|^4.
$$

In particular the charge in $\psi^*\phi^2$ is $-2e+2e=0$, which uses the stated charge ratio. The potential is real, bounded below and has the zero-field minimum, while the kinetic terms have the standard positive signs. A complete example is therefore

$$
\boxed{\mathcal L_2=-\frac14f_{\mu\nu}f^{\mu\nu}
+(D_\mu\phi)^*D^\mu\phi+(D_\mu\psi)^*D^\mu\psi-V(\phi,\psi).}
$$

There is genuine direct interaction even with $g=0$ because $b\ne0$. In four spacetime dimensions $b$ has [mass dimension](../../../../../mass-dimension.md) $-1$, but the expanded potential contains only quadratic, cubic and quartic field monomials; the cubic coefficient $M^2b$ has dimension one. Thus the example is also power-counting renormalizable.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
