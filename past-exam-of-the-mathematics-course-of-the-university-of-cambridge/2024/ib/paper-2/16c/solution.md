<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

A gauge transformation is

$$
\boxed{A_\mu\longmapsto A_\mu+\partial_\mu\chi}.
$$

Because [partial derivatives](../../../../../partial-derivative.md) commute, the added contribution to $F_{\mu\nu}$ is

$$
\partial_\mu\partial_\nu\chi-\partial_\nu\partial_\mu\chi=0,
$$

so the [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) is gauge invariant.

Define

$$
E=-\nabla\Phi-\partial_tA,
\qquad
B=\nabla\times A.
$$

Since $\partial_0=c^{-1}\partial_t$ and $A_0=-\Phi/c$,

$$
\boxed{F_{0i}=-\frac{E_i}{c},
\qquad
F_{i0}=\frac{E_i}{c},
\qquad
F_{ij}=\epsilon_{ijk}B_k}.
$$

The identity

$$
\partial_\lambda F_{\mu\nu}
+\partial_\mu F_{\nu\lambda}
+\partial_\nu F_{\lambda\mu}=0
$$

follows directly from $F=dA$. Its spatial and mixed components are

$$
\nabla\cdot B=0,
\qquad
\nabla\times E=-\partial_tB.
$$

For the other two equations define the four-current

$$
\boxed{j^\mu=(c\rho,J)}.
$$

Then $\partial_\nu F^{0\nu}=\mu_0j^0$ gives

$$
\nabla\cdot E=\mu_0c^2\rho=\frac\rho{\epsilon_0},
$$

and $\partial_\nu F^{i\nu}=\mu_0j^i$ gives

$$
\nabla\times B-\frac1{c^2}\partial_tE=\mu_0J.
$$

This is the [Covariant Maxwell equation with the minus-plus-plus-plus metric](../../../../../covariant-maxwell-equation-with-the-minus-plus-plus-plus-metric.md).

Using

$$
F^{\rho\sigma}F_{\rho\sigma}
=2\left(B^2-\frac{E^2}{c^2}\right),
$$

one finds

$$
\boxed{
T^{00}=\frac1{2\mu_0}
\left(B^2+\frac{E^2}{c^2}\right)
=\frac12\left(\frac{B^2}{\mu_0}+\epsilon_0E^2\right)}.
$$

This is the electromagnetic energy density.

For a null [vector](../../../../../vector.md), the trace term in $T^{\mu\nu}k_\mu k_\nu$ vanishes. Put

$$
q^\rho=k_\mu F^{\mu\rho}.
$$

Antisymmetry gives $q\cdot k=0$. A [vector](../../../../../vector.md) orthogonal to a null [vector](../../../../../vector.md) has nonnegative Minkowski norm, so

$$
T^{\mu\nu}k_\mu k_\nu=\frac1{\mu_0}q^\rho q_\rho\geq0.
$$

Explicitly, in a frame with $k^\mu=\kappa(1,1,0,0)$,

$$
q^2=\kappa^2\left[
\left(B_3-\frac{E_2}{c}\right)^2
+\left(B_2+\frac{E_3}{c}\right)^2
\right].
$$

Hence the [null energy condition for the electromagnetic field](../../../../../null-energy-condition-for-the-electromagnetic-field.md) is strict whenever the contraction is nonzero:

$$
\boxed{T^{\mu\nu}k_\mu k_\nu>0}.
$$

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
