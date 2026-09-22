<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use the free [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) and the [canonical commutation relations](../../../../../../canonical-commutation-relation.md). The kinetic momentum term gives

$$
[H_1,\phi_1(t,\mathbf x)]
=\frac12\int d^3y\,[\pi_1(t,\mathbf y)^2,\phi_1(t,\mathbf x)]
=-i\pi_1(t,\mathbf x).
$$

The [Heisenberg picture](../../../../../../heisenberg-picture.md) equation therefore yields $\dot\phi_1=\pi_1$.

For the momentum commutator, the mass term gives $im_1^2\phi_1(\mathbf x)$. The gradient term gives

$$
\frac12\int d^3y\,[(\nabla\phi_1(\mathbf y))^2,\pi_1(\mathbf x)]
=i\int d^3y\,\nabla\phi_1(\mathbf y)\cdot\nabla_{\mathbf y}\delta^{(3)}(\mathbf y-\mathbf x)
=-i\nabla^2\phi_1(\mathbf x),
$$

where [integration by parts](../../../../../../integration-by-parts.md) differentiates the field instead of the [Dirac delta distribution](../../../../../../dirac-delta-function.md). Thus

$$
[H_1,\pi_1]=i(m_1^2-\nabla^2)\phi_1,\qquad
\dot\pi_1=(\nabla^2-m_1^2)\phi_1.
$$

Combining the two first-order operator equations gives the [Klein-Gordon equation](../../../../../../klein-gordon-equation.md):

$$
\boxed{(\partial_t^2-\nabla^2+m_1^2)\phi_1=(\Box+m_1^2)\phi_1=0.}
$$

Suitable decay or spatial smearing removes the boundary term in the integration by parts.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
