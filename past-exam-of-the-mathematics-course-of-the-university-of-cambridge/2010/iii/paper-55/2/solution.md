<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Absorb the gauge coupling into a matrix-valued [connection 1-form](../../../../../connection-1-form-split.md), and use

$$
F=dA+A\wedge A,qquad
D\alpha=d\alpha+A\wedge\alpha-(-1)^p\alpha\wedge A
$$

for an adjoint-valued $p$-form $\alpha$. The [matrix trace](../../../../../matrix-trace.md) supplies the usual invariant nondegenerate pairing of the [Lie algebra](../../../../../lie-algebra-split.md), and the spacetime metric defining the [Hodge star](../../../../../hodge-star-operator.md) is fixed during the gauge-field variation. Since $\delta F=D\delta A$ and the two-form Hodge pairing is symmetric,

$$
\begin{aligned}
\delta I
&=2\int_M\operatorname{tr}(D\delta A\wedge *F)\\
&=2\int_{\partial M}\operatorname{tr}(\delta A\wedge *F)
+2\int_M\operatorname{tr}(\delta A\wedge D*F).
\end{aligned}
$$

For variations fixed at the boundary, the [Yang-Mills equations](../../../../../yang-mills-equations.md) are therefore

$$
\boxed{D*F=0.}
$$

They accompany, rather than replace, the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) $DF=0$, which follows directly by substituting $F=dA+A\wedge A$ and using $d^2=0$.

Fix the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) convention

$$
A^g=g^{-1}Ag+g^{-1}dg,qquad F^g=g^{-1}Fg.
$$

Taking $g=1+\eta+O(\eta^2)$ gives

$$
\boxed{\delta_\eta A=d\eta+[A,\eta]=D\eta,qquad
\delta_\eta F=[F,\eta].}
$$

The curvature variation also follows from $D(D\eta)=[F,\eta]$. If the group parameter is defined with the opposite sign, both displayed infinitesimal variations change sign together.

The [Hodge star](../../../../../hodge-star-operator.md) acts only on spacetime indices, so $\delta(*F)=[*F,\eta]$. Consequently

$$
\begin{aligned}
\delta_\eta\operatorname{tr}(*F\wedge F)
&=\operatorname{tr}([*F,\eta]\wedge F+*F\wedge[F,\eta])\\
&=\operatorname{tr}([*F\wedge F,\eta])=0.
\end{aligned}
$$

This proves **exact off-shell [gauge invariance](../../../../../gauge-invariance.md), with no surviving boundary term**, even for a gauge parameter nonzero at the boundary. It does not require the [Yang-Mills equations](../../../../../yang-mills-equations.md).

One can check the surface terms explicitly in the integrated variation. The Lie-algebra-valued four-form $[F,*F]=F\wedge *F-*F\wedge F$ vanishes: writing $F=F^iT_i$, the coefficients $F^i\wedge *F^j$ are symmetric in $i,j$, and multiply the antisymmetric commutator $[T_i,T_j]$. Thus $D^2*F=[F,*F]=0$, and the gauge substitution in the variation gives

$$
\delta_\eta I=2\int_{\partial M}\operatorname{tr}(D\eta\wedge *F+\eta D*F)
=2\int_{\partial M}d\operatorname{tr}(\eta *F)=0.
$$

The last equality is [Stokes theorem](../../../../../stokes-theorem.md) on the closed boundary; equivalently the cancellation is already pointwise in the preceding derivation. Keeping only the first surface term from an arbitrary variation would incorrectly produce a gauge boundary term.

For the additional [Yang-Mills theta term](../../../../../yang-mills-theta-term.md), denote its coefficient-free integral by $P=\int_M\operatorname{tr}(F\wedge F)$. Its gauge variation is again pointwise zero:

$$
\delta_\eta\operatorname{tr}(F\wedge F)=\operatorname{tr}([F\wedge F,\eta])=0.
$$

Under an arbitrary connection variation, its [boundary variation of the Yang-Mills theta term](../../../../../boundary-variation-of-the-yang-mills-theta-term.md) is

$$
\begin{aligned}
\delta P
&=2\int_M\operatorname{tr}(D\delta A\wedge F)\\
&=2\int_{\partial M}\operatorname{tr}(\delta A\wedge F)
+2\int_M\operatorname{tr}(\delta A\wedge DF)
=2\int_{\partial M}\operatorname{tr}(\delta A\wedge F).
\end{aligned}
$$

The bulk term vanishes by the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md). Therefore **adding a constant multiple of $P$ does not change the bulk [Yang-Mills equations](../../../../../yang-mills-equations.md)**. With fixed boundary potential, it also leaves the usual variational problem unchanged. If boundary variations are allowed, it changes the boundary term: $I+\kappa P$ has surface variation $2\int_{\partial M}\operatorname{tr}(\delta A\wedge(*F+\kappa F))$, so compatible boundary conditions or a boundary action must account for that change.

Locally $\operatorname{tr}(F\wedge F)=d\operatorname{tr}(A\wedge dA+\tfrac23 A\wedge A\wedge A)$, the unnormalized [Chern-Simons 3-form](../../../../../chern-simons-3-form.md) identity. That three-form need not be globally defined on a nontrivial bundle, so absence of a bulk variation does not force $P$ itself to vanish. Its exact [gauge invariance](../../../../../gauge-invariance.md) is the curvature-conjugation calculation above, independently of the choice of local gauge potential.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
