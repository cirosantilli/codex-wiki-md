<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Normalize the [generating functional](../../../../../generating-functional.md) by its value with all sources zero, and take the connected part of the [time-ordered correlation function](../../../../../time-ordered-correlation-function.md). Source differentiation of the interaction exponential is equivalent to the [Dyson series](../../../../../dyson-series.md) followed by [Wick's theorem](../../../../../wick-s-theorem.md). Write $D(x-y)=\langle T\phi(x)\phi(y)\rangle_0$ and $F_{ij}(x-y)=\langle T\psi_i(x)\bar\psi_j(y)\rangle_0$ temporarily, so that every contraction has an unambiguous meaning.

The second-order [Dyson series](../../../../../dyson-series.md) contributes

$$
\frac{(ig)^2}{2!}\int d^4x\,d^4y\,
\langle T\phi(x_a)\phi(y_a)\phi(x)\phi(y)
[\bar\psi_i(x)\psi_i(x)][\bar\psi_j(y)\psi_j(y)]\rangle_{0,c}.
$$

There are two connected external [scalar field](../../../../../scalar-field.md) attachments:

$$
D(x_a-x)D(y_a-y)+D(x_a-y)D(y_a-x).
$$

They become equal after exchanging the integration variables $x,y$, cancelling $2!$. The connected [fermion](../../../../../fermion.md) contractions have the [closed fermion loop sign](../../../../../closed-fermion-loop-sign.md):

$$
\langle T[\bar\psi_i(x)\psi_i(x)][\bar\psi_j(y)\psi_j(y)]\rangle_{0,c}
=-F_{ij}(x-y)F_{ji}(y-x)
=-\operatorname{tr}[F(x-y)F(y-x)].
$$

The minus sign can also be checked directly: the pairing of the first with the fourth field and the second with the third has positive pairing parity, but $\langle T\bar\psi_i(x)\psi_j(y)\rangle=-F_{ji}(y-x)$. Multiplying it by $(ig)^2=-g^2$ leaves a positive result:

$$
G_c^{(2)}(x_a,y_a)=g^2\int d^4x\,d^4y\,
D(x_a-x)D(y_a-y)\operatorname{tr}[F(x-y)F(y-x)].
$$

A contraction of the two external fields with each other times a [vacuum bubble](../../../../../vacuum-feynman-diagram.md) cancels against the normalization. Separate [fermion](../../../../../fermion.md) [tadpole integrals](../../../../../tadpole-integral.md) at $x$ and $y$ belong to a product of one-point functions, removed by taking the connected part.

To match the source's [generating functional](../../../../../generating-functional.md) convention, distinguish its displayed kernels from contractions. The positive $iJ\Delta J/2$ exponent gives $D=-i\Delta$. With the source insertion order in equation (5), the positive $i\bar\eta S_F\eta$ exponent similarly gives $F=-iS_F$. The two [scalar propagators](../../../../../scalar-propagator.md) and two [Dirac propagators](../../../../../dirac-propagator.md) supply a total phase $(-i)^4=1$. Thus, writing $S=S_F$ as in the requested formula,

$$
\boxed{G_c^{(2)}(x_a,y_a)=g^2\int d^4x\,d^4y\,
\Delta(x_a-x)\Delta(y_a-y)\operatorname{tr}[S(x-y)S(y-x)].}
$$

The [matrix trace](../../../../../matrix-trace.md) closes the [spinor](../../../../../spinor.md) indices; no extra factor of two or additional [symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) remains for a [Dirac field](../../../../../dirac-field.md) with this [Yukawa interaction](../../../../../yukawa-interaction.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
