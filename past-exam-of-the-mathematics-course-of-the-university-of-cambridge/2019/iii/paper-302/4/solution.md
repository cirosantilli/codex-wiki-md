<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $G$ be a simple [Lie group](../../../../../lie-group.md), let $T^a$ be Hermitian matrices for a finite-dimensional [unitary representation](../../../../../unitary-representation.md) $R$, and normalize

$$
[T^a,T^b]=if^{ab}{}_cT^c,
\qquad \operatorname{tr}(T^aT^b)=T(R)\delta^{ab}.
$$

A matter field $\psi$ transforms locally as $\psi'(x)=U(x)\psi(x)$, where $U(x)=e^{ig\epsilon^a(x)T^a}$. An ordinary derivative of $\psi$ does not transform covariantly because it differentiates $U$. Introduce a [gauge field](../../../../../gauge-field.md) $A_\mu=A_\mu^aT^a$ and the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md)

$$
D_\mu=\partial_\mu-igA_\mu.
$$

Demanding $D_\mu'\psi'=U D_\mu\psi$ determines the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md)

$$
A_\mu'=UA_\mu U^{-1}-\frac{i}{g}(\partial_\mu U)U^{-1}.
$$

To first order in $\epsilon$,

$$
\boxed{\delta A_\mu=\partial_\mu\epsilon+ig[\epsilon,A_\mu],
\qquad
\delta A_\mu^a=\partial_\mu\epsilon^a+g f^{bc}{}_aA_\mu^b\epsilon^c.}
$$

The [gauge field strength](../../../../../gauge-field-strength.md) is defined by $[D_\mu,D_\nu]=-igF_{\mu\nu}$:

$$
F_{\mu\nu}
=\partial_\mu A_\nu-\partial_\nu A_\mu-ig[A_\mu,A_\nu],
$$

or, in components,

$$
F_{\mu\nu}^a
=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a
+g f^{bc}{}_aA_\mu^bA_\nu^c.
$$

Covariance of the commutator gives

$$
F_{\mu\nu}'=UF_{\mu\nu}U^{-1},
\qquad
\delta F_{\mu\nu}=ig[\epsilon,F_{\mu\nu}].
$$

The commutator term distinguishes [Yang-Mills theory](../../../../../yang-mills-theory.md) from an [Abelian gauge theory](../../../../../abelian-gauge-theory.md) and produces cubic and quartic gauge-boson interactions.

For a [Dirac field](../../../../../dirac-field.md) of mass $m$ in $R$, the Lagrangian is

$$
\boxed{\mathcal L
=-\frac14F_{\mu\nu}^aF^{a\mu\nu}
+\bar\psi(i\gamma^\mu D_\mu-m)\psi.}
$$

Equivalently, the gauge term is proportional to $-\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})$. The [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md) and $F'_{\mu\nu}=UF_{\mu\nu}U^{-1}$ make it invariant. Unitarity gives $\bar\psi'=\bar\psi U^{-1}$, while $D_\mu'\psi'=UD_\mu\psi$, so both the matter kinetic term and mass term are invariant. A complex scalar $\phi$ in a unitary representation may instead be coupled through

$$
\mathcal L_\phi=(D_\mu\phi)^\dagger D^\mu\phi-V(\phi),
$$

provided the [scalar potential](../../../../../scalar-potential.md) $V$ is $G$-invariant.

The simplicity assumption means that the [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g$ is nonabelian and has no proper nonzero [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). Its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) is therefore irreducible, and every invariant symmetric bilinear form is proportional to the [Killing form](../../../../../killing-form.md). Consequently the pure gauge kinetic term has one overall [gauge coupling](../../../../../gauge-coupling.md) for a simple factor. The theory has no independent Abelian gauge direction; if the gauge algebra were a direct sum of simple and Abelian ideals, each factor could instead carry its own coupling. A simple group may still have a discrete center, but this does not add a gauge boson because gauge bosons are indexed by the Lie algebra.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
