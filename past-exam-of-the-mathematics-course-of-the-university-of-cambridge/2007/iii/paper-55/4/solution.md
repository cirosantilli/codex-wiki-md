<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use an unfluxed toroidal zero-mode [dimensional reduction](../../../../../dimensional-reduction.md), with no projection removing fields. A ten-dimensional [gauge field](../../../../../gauge-field.md) has $10-2=8$ physical polarizations per [gauge generator](../../../../../gauge-generator.md). Its [Majorana-Weyl spinor](../../../../../majorana-weyl-spinor.md) partner has sixteen real components before the massless equation, and eight propagating fermionic states. Thus [ten-dimensional super Yang-Mills theory](../../../../../ten-dimensional-super-yang-mills-theory.md) has sixteen real [supercharges](../../../../../supersymmetry-generator.md) and eight bosonic plus eight fermionic states per generator.

Split the spacetime index as $M=(\mu,m)$, with $\mu=0,\ldots,3$ and six internal directions. The zero modes of $A_M$ become $A_\mu$ and six real adjoint [scalar fields](../../../../../scalar-field.md) $X_m=A_m$. The [spinor representation](../../../../../spin-representation.md) decomposes under $\operatorname{Spin}(1,3)\times\operatorname{Spin}(6)$ into four four-dimensional [Weyl spinors](../../../../../weyl-spinor.md); the Majorana condition supplies their conjugates rather than independent additional spinors. All sixteen [supercharges](../../../../../supersymmetry-generator.md) survive, giving [four-dimensional N=4 super Yang-Mills theory](../../../../../four-dimensional-n-4-super-yang-mills-theory.md). The [supermultiplet](../../../../../supermultiplet.md) is therefore **one gauge vector, four Weyl [gauginos](../../../../../gaugino.md) and six real scalars, all in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md)**, with $2+6=8$ bosonic and $4\times2=8$ fermionic states. The internal $\operatorname{Spin}(6)\simeq SU(4)$ acts as [R-symmetry](../../../../../r-symmetry.md), with the scalars in its six-dimensional representation and the Weyl [gauginos](../../../../../gaugino.md) in its four-dimensional representation.

Since the internal derivatives vanish, the internal [Yang-Mills field strength](../../../../../gauge-field-strength.md) is $F_{mn}=-ig_4[X_m,X_n]$ in a Hermitian-generator convention. The internal part of the gauge [kinetic term](../../../../../kinetic-term.md) becomes the [scalar potential](../../../../../scalar-potential.md)

$$
\boxed{V=\frac{g_4^2}{4}\sum_{m,n,a}(f^{abc}X_m^bX_n^c)^2=\frac{g_4^2}{4}\sum_{m,n}\operatorname{tr}\bigl([X_m,X_n]^\dagger[X_m,X_n]\bigr).}
$$

Here the invariant [trace](../../../../../matrix-trace.md) is normalized by $\operatorname{tr}(T^aT^b)=\delta^{ab}$ and $[T^a,T^b]=if^{abc}T^c$; the coupling and scalar [kinetic terms](../../../../../kinetic-term.md) use the same normalization. The sum includes both orders of each pair. For Hermitian $X_m$, the [commutator](../../../../../commutator.md) is anti-Hermitian, so equivalently $V=-\frac{g_4^2}{4}\sum_{m,n}\operatorname{tr}[X_m,X_n]^2$. It is nonnegative and vanishes exactly when all six adjoint scalars commute. This gives the classical [vacuum moduli space of a supersymmetric gauge theory](../../../../../vacuum-moduli-space-of-a-supersymmetric-gauge-theory.md).

Interpret $A_{MNP}$ as a massless three-form [gauge field](../../../../../gauge-field.md), with transformation $A_3\mapsto A_3+d\Lambda_2$ and [kinetic term](../../../../../kinetic-term.md) built from $F_4=dA_3$. The [massless p-form gauge field](../../../../../massless-p-form-gauge-field.md) count is an on-shell count, rather than the raw $\binom D3$ [tensor](../../../../../tensor.md) components. For a null plane wave, [gauge transformations](../../../../../gauge-transformation.md) remove the components along the null gauge direction, while the field equation removes the complementary longitudinal components. The independent polarization is consequently an antisymmetric [tensor](../../../../../tensor.md) on the $D-2$ transverse directions. Thus

$$
\boxed{n_3(D)=\binom{D-2}{3}.}
$$

This argument incorporates the redundancies in the two-form gauge parameter; subtracting $\binom D2$ once from $\binom D3$ would not do so.

Let $n=D-4$ and split indices into four-dimensional and internal ones. The [toroidal reduction of a p-form gauge field](../../../../../toroidal-reduction-of-a-p-form-gauge-field.md) gives one $A_{\mu\nu\rho}$, $n$ two-forms $A_{\mu\nu i}$, $\binom n2$ vectors $A_{\mu ij}$ and $\binom n3$ scalars $A_{ijk}$. A massless three-form in four dimensions has no local propagating state; each massless two-form has one, each vector two and each scalar one. The two-form state can equivalently be represented by a scalar using [massless p-form duality](../../../../../massless-p-form-duality.md): its three-form field strength satisfies $H_3=*da$. Consequently

$$
\begin{aligned}
n_{\mathrm{4D}}&=0+n+2\binom n2+\binom n3\\
&=n+n(n-1)+\frac{n(n-1)(n-2)}6\\
&=\frac{n(n+1)(n+2)}6=\binom{D-2}{3}.
\end{aligned}
$$

This verifies the required matching, including $D=6$ where the count is $2+2=4$. The [nondynamical four-dimensional three-form](../../../../../nondynamical-four-dimensional-three-form.md) can carry a constant flux parameter, but that is not an additional propagating [degree of freedom](../../../../../degree-of-freedom.md).

[Eleven-dimensional supergravity](../../../../../eleven-dimensional-supergravity.md) contains the metric $G_{MN}$, a three-form $A_{MNP}$ and a Majorana [gravitino](../../../../../gravitino.md) $\Psi_M$. The massless graviton is a symmetric traceless [tensor](../../../../../tensor.md) of the nine-dimensional transverse rotation group, giving $9\times10/2-1=44$ states. The three-form gives $\binom93=84$. The [gravitino](../../../../../gravitino.md) is a gamma-traceless transverse vector-spinor: a [spinor representation](../../../../../spin-representation.md) of $\operatorname{Spin}(9)$ has sixteen real components, so it gives $9\times16-16=128$ states. Hence the eleven-dimensional balance is $44+84=128$ bosonic states and $128$ fermionic states.

Reduction on a circle yields [type IIA supergravity](../../../../../type-iia-supergravity.md), with thirty-two real [supercharges](../../../../../supersymmetry-generator.md) and opposite ten-dimensional chiralities. The metric decomposes into the ten-dimensional metric, the [Kaluza-Klein](../../../../../kaluza-klein-theory.md) vector $C_\mu=G_{\mu\,11}$ and the radius scalar, or dilaton. Their counts are $35+8+1=44$. The three-form gives a ten-dimensional three-form $C_{\mu\nu\rho}$ and a two-form $B_{\mu\nu}=A_{\mu\nu\,11}$, with $\binom83+\binom82=56+28=84$ states. The eleven-dimensional [Majorana spinor](../../../../../majorana-spinor.md) decomposes into two opposite-chirality [Majorana-Weyl spinors](../../../../../majorana-weyl-spinor.md). The external [gravitino](../../../../../gravitino.md) components give two [gravitini](../../../../../gravitino.md), each with $8\times8-8=56$ states; the internal component supplies two spin-one-half dilatini, each with eight states. Therefore

$$
\boxed{\text{10D IIA: }35+8+1+56+28=128,\qquad2\times56+2\times8=128.}
$$

The two-form is in the NS--NS sector and the one-form and three-form are the Ramond--Ramond potentials. This reduction is nonchiral IIA rather than IIB.

Reduction on a seven-torus yields [four-dimensional N=8 supergravity](../../../../../four-dimensional-n-8-supergravity.md), again preserving thirty-two real [supercharges](../../../../../supersymmetry-generator.md). From $G_{MN}$ one gets one graviton, seven vectors $G_{\mu i}$ and $7\times8/2=28$ scalars $G_{ij}$, giving $2+7\times2+28=44$ states. From $A_{MNP}$ one gets a nonpropagating four-dimensional three-form, seven two-forms, $\binom72=21$ vectors and $\binom73=35$ scalars, giving $0+7+21\times2+35=84$ states. Dualizing the seven two-forms to scalars gives the familiar field content

$$
\boxed{\text{4D: one graviton, }28\text{ vectors, }70\text{ real scalars};\qquad2+28\times2+70=128.}
$$

The [gravitino](../../../../../gravitino.md) reduces to eight four-dimensional Majorana [gravitini](../../../../../gravitino.md) and $7\times8=56$ spin-one-half Majorana fermions, after the external [gravitini](../../../../../gravitino.md) are separated from their gamma-trace mixing with the internal components. Their count is $8\times2+56\times2=128$. Together these fields form the single maximal [supergravity multiplet](../../../../../supergravity-multiplet.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
