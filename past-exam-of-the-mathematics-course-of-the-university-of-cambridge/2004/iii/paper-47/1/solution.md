<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a Minkowski [external source](../../../../../source-quantum-field-theory.md) term $+\int J\chi$, where $\chi$ is the integration variable, and normalize the vacuum functional:

$$
Z[J]=\frac{\int\mathcal D\chi\,\exp\{iS[\chi]+i\int d^4x\,J(x)\chi(x)\}}
{\int\mathcal D\chi\,e^{iS[\chi]}},\qquad W[J]=\log Z[J].
$$

The usual vacuum boundary prescription is implicit. This is the logarithmic convention $Z=e^W$ for the [connected generating functional](../../../../../connected-generating-functional.md). It makes the given quadratic expression consistent with $\Delta_F=\langle T\chi\chi\rangle$. Another common convention is $Z=e^{iW_c}$, with $W_c=-iW$; mixing the two conventions would change the factors of $i$ below.

[Functional derivative](../../../../../functional-derivative.md) generates the full and connected [correlation functions](../../../../../correlation-function.md):

$$
G_n(x_1,\ldots,x_n)=\left.i^{-n}\frac{\delta^n Z}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0},
\qquad
G_n^c(x_1,\ldots,x_n)=\left.i^{-n}\frac{\delta^n W}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.
$$

These are [time-ordered products](../../../../../time-ordered-product.md) in the vacuum, and $G_1=G_1^c=0$ by the stated assumption. Differentiating $e^W$ four times partitions the four insertions into connected blocks. All partitions with a singleton vanish, leaving

$$
\boxed{G_4(1,2,3,4)=G_4^c(1,2,3,4)
+G_2^c(1,2)G_2^c(3,4)
+G_2^c(1,3)G_2^c(2,4)
+G_2^c(1,4)G_2^c(2,3).}
$$

The shorthand arguments stand for [spacetime](../../../../../spacetime.md) points; this is a functional cumulant identity, not an assumption of a free field.

To construct the [quantum effective action](../../../../../effective-action.md), define the source-dependent classical field

$$
\varphi(x)=\langle\chi(x)\rangle_J=-i\frac{\delta W}{\delta J(x)}.
$$

Locally invert this relation to obtain $J[\varphi]$, assuming the response [integral kernel](../../../../../integral-kernel.md) is invertible with the chosen regulator and boundary prescription. Take its [Legendre transform](../../../../../convex-conjugate.md)

$$
\boxed{i\Gamma[\varphi]=W[J[\varphi]]-i\int d^4x\,J[\varphi](x)\varphi(x).}
$$

The chain-rule terms proportional to $\delta J$ cancel, so $\delta\Gamma/\delta\varphi=-J$. A field-independent constant is fixed separately and is immaterial to the vertices. At zero [external source](../../../../../source-quantum-field-theory.md) the classical field is zero, and there is no linear term.

For the two-point vertex, differentiate the classical field once. If $G=G_2^c$, then

$$
\frac{\delta\varphi(x)}{\delta J(y)}=iG(x,y),\qquad
\frac{\delta J(x)}{\delta\varphi(y)}=-iG^{-1}(x,y),
\qquad
\int d^4z\,G(x,z)G^{-1}(z,y)=\delta^{(4)}(x-y).
$$

The vertex coefficients in this problem are [derivatives](../../../../../derivative.md) of $i\Gamma$, not of $\Gamma$ alone. Therefore

$$
\boxed{\Gamma_2(x,y)=-G^{-1}(x,y).}
$$

For the three-point vertex, the [derivative](../../../../../derivative.md) of the connected two-point [integral kernel](../../../../../integral-kernel.md) at a general [external source](../../../../../source-quantum-field-theory.md) is

$$
\frac{\delta G(a,b)}{\delta J(c)}=iG_3^c(a,b,c).
$$

Combine this with $\delta J/\delta\varphi=-iG^{-1}$ and differentiate the inverse identity, $\delta G^{-1}=-G^{-1}(\delta G)G^{-1}$. This gives the [logarithmic-source inverse-kernel vertices](../../../../../logarithmic-source-inverse-kernel-vertices.md) relation

$$
\boxed{\Gamma_3(x,y,z)=\int d^4a\,d^4b\,d^4c\,
G^{-1}(x,a)G^{-1}(y,b)G^{-1}(z,c)G_3^c(a,b,c).}
$$

All kernels here are finally evaluated at zero [external source](../../../../../source-quantum-field-theory.md). The connected three-point function is amputated by its three inverse [quantum field theory propagators](../../../../../propagator.md).

For the specified quadratic $W$, the [external source](../../../../../source-quantum-field-theory.md) response is $\varphi=i\Delta_FJ$, hence $J=-i\Delta_F^{-1}\varphi$. Substitution in the transform gives

$$
\boxed{\Gamma[\varphi]=\frac i2\int d^4x\,d^4y\,
\varphi(x)\Delta_F^{-1}(x-y)\varphi(y),\qquad
\Gamma_2=-\Delta_F^{-1},\qquad\Gamma_n=0\ (n\geq3).}
$$

For the standard free [quantum field theory propagator](../../../../../propagator.md) $\widetilde\Delta_F(p)=i/(p^2-m^2+i0)$, this is the usual quadratic free action, up to the vacuum prescription. The [generating functional](../../../../../generating-functional.md) is Gaussian, so connected functions beyond second order vanish and there are no interaction vertices or nontrivial [scattering amplitudes](../../../../../scattering-amplitude.md). Full higher even-point functions can still be nonzero: they are products of two-point functions, as the four-point formula shows.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
