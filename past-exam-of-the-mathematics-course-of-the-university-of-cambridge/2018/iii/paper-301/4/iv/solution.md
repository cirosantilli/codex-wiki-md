<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the [active Lorentz transformation of a vector field](../../../../../../active-lorentz-transformation-of-a-vector-field.md), coordinates are held fixed and $A'^\mu(x)=\Lambda^\mu{}_{\nu}A^\nu(\Lambda^{-1}x)$. Its field strength transforms as a two-index [Lorentz tensor](../../../../../../lorentz-tensor.md). The index contractions in the [Maxwell Lagrangian](../../../../../../maxwell-lagrangian.md) are invariant by $\Lambda^T\eta\Lambda=\eta$, so the density transforms as a [Lorentz scalar](../../../../../../lorentz-scalar.md):

$$
\mathcal L'(x)=\mathcal L(\Lambda^{-1}x).
$$

For $\Lambda=I+\alpha\omega$, its inverse is $I-\alpha\omega+O(\alpha^2)$. Expanding the coordinate argument therefore gives

$$
\boxed{\delta\mathcal L(x)=-\alpha\omega^\mu{}_{\nu}x^\nu\partial_\mu\mathcal L(x).}
$$

Set $v^\mu(x)=\alpha\omega^\mu{}_{\nu}x^\nu$. Part (iii) implies $\partial_\mu v^\mu=\alpha\omega^\mu{}_{\mu}=0$. The product rule then converts the variation into a total derivative:

$$
\boxed{\delta\mathcal L=-\partial_\mu\bigl(\alpha\omega^\mu{}_{\nu}x^\nu\mathcal L\bigr).}
$$

Its integral changes the action only by a boundary term, which is the condition needed for [Noether's theorem](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
