<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Chern number](../../../../../chern-number.md) turns local curvature data into a global integer. Let $E\to M$ be a complex [vector bundle](../../../../../vector-bundle.md) over a compact oriented manifold without boundary, with a [unitary connection](../../../../../unitary-connection.md) represented locally by an anti-Hermitian matrix-valued one-form $A$. Its [curvature form of a connection](../../../../../curvature-form.md) is $F=dA+A\wedge A$. The [Chern-Weil theory](../../../../../chern-weil-homomorphism.md) representative of the total [Chern class](../../../../../chern-class.md) is

$$
c(E,A)=\det\left(I+\frac{iF}{2\pi}\right)=1+c_1(E,A)+c_2(E,A)+\cdots.
$$

The coefficients are [closed differential forms](../../../../../closed-differential-form.md). They represent the images of integral [Chern classes](../../../../../chern-class.md) in [de Rham cohomology](../../../../../de-rham-cohomology.md). On an oriented $2r$-manifold, a product $c_{i_1}\cdots c_{i_s}$ with $i_1+\cdots+i_s=r$ pairs with the [fundamental class](../../../../../fundamental-class.md) to give a [Chern number](../../../../../chern-number.md), an integer independent of the [unitary connection](../../../../../unitary-connection.md).

For example,

$$
c_1=\frac{i}{2\pi}\operatorname{Tr}F,\qquad
c_2=\frac1{8\pi^2}\left\{\operatorname{Tr}(F\wedge F)-\operatorname{Tr}F\wedge\operatorname{Tr}F\right\}.
$$

For an $SU(N)$ bundle with $N\geq2$, $\operatorname{Tr}F=0$. On an oriented four-manifold the [Second Chern number](../../../../../second-chern-number.md) is then

$$
\boxed{q=\int_M c_2=\frac1{8\pi^2}\int_M\operatorname{Tr}(F\wedge F)\in\mathbb Z,}
$$

using the fundamental [matrix trace](../../../../../matrix-trace.md) and the stated anti-Hermitian convention. The trace-product correction is required for a general $U(N)$ bundle; it cannot simply be omitted. The sign of a physical [instanton number](../../../../../instanton-number.md) also depends on the trace and [orientation](../../../../../orientation-of-a-simplex.md) convention, so these conventions must accompany the formula.

The local origin of closure is the [Bianchi identity](../../../../../bianchi-identity.md) $D_AF=0$ and the cyclic [matrix trace](../../../../../matrix-trace.md): $d\operatorname{Tr}(F\wedge F)=0$. Independence of the [connection one-form](../../../../../connection-one-form.md) follows more concretely by varying a family $A_t$. Since $\dot F_t=D_{A_t}\dot A_t$, the [Chern-Weil connection transgression](../../../../../chern-weil-connection-transgression.md) is

$$
\frac{d}{dt}\operatorname{Tr}(F_t\wedge F_t)=2\,d\operatorname{Tr}(\dot A_t\wedge F_t).
$$

Its integral on a closed four-manifold is zero by the [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md). This proves connection independence of $q$; the integrality is the global [Chern class](../../../../../chern-class.md) statement, not merely a consequence of the local formula.

The local primitive of the [Second Chern form](../../../../../second-chern-form.md) is the [Chern-Simons three-form](../../../../../chern-simons-3-form.md)

$$
\boxed{Y(A)=\frac1{8\pi^2}\operatorname{Tr}\left(A\wedge dA+\frac23A\wedge A\wedge A\right),\qquad dY=c_2.}
$$

Here we continue to use $SU(N)$, so $c_2=\operatorname{Tr}(F\wedge F)/(8\pi^2)$. The cubic coefficient is forced by the [exterior derivative](../../../../../exterior-derivative.md). In the graded cyclic [matrix trace](../../../../../matrix-trace.md), $d\operatorname{Tr}(A^3)=3\operatorname{Tr}(dA\wedge A^2)$ and $\operatorname{Tr}(A^4)=0$, the latter because cycling one degree-one factor past the other three changes its sign. Therefore

$$
d\operatorname{Tr}(A\wedge dA+\tfrac23A^3)
=\operatorname{Tr}(dA\wedge dA+2dA\wedge A^2)
=\operatorname{Tr}(F\wedge F).
$$

Matrix-valued [differential forms](../../../../../differential-form-split.md) require both matrix order and the graded signs; treating all factors as commuting scalars would lose this derivation.

The [Chern-Simons three-form](../../../../../chern-simons-3-form.md) depends on a local trivialization and is not itself gauge-invariant. For the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) convention $A^g=g^{-1}Ag+g^{-1}dg$, set $u=g^{-1}dg$. The [gauge change of the Chern-Simons three-form](../../../../../gauge-change-of-the-chern-simons-three-form.md) is

$$
Y(A^g)=Y(A)-\frac1{8\pi^2}d\operatorname{Tr}(dg\,g^{-1}\wedge A)
-\frac1{24\pi^2}\operatorname{Tr}(u\wedge u\wedge u).
$$

The last term is closed by the [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md). On a closed three-manifold its integral is an integer with the fundamental $SU(N)$ normalization. Consequently **the Chern-Simons integral is naturally defined modulo integers**, while its exponential $\exp(2\pi i\ell\int Y)$ is invariant under large [Yang-Mills gauge transformations](../../../../../yang-mills-gauge-transformation.md) for integer level $\ell$.

This also explains why a nonzero [Chern number](../../../../../chern-number.md) is compatible with $dY=c_2$: $Y$ need not be a globally defined three-form. On $S^4$, trivialize over two hemispheres and let $A_N=A_S^g$ on their common equator $\Sigma=S^3$, oriented as the boundary of the northern hemisphere. The [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) and the gauge-change formula give

$$
q=\int_\Sigma(Y(A_N)-Y(A_S))
=-\frac1{24\pi^2}\int_\Sigma\operatorname{Tr}(g^{-1}dg)^3.
$$

For $SU(2)\cong S^3$, this is the degree of the transition map, with compatible group [orientation](../../../../../orientation-of-a-simplex.md); for $SU(N)$ it is the corresponding integer in $\pi_3(SU(N))$. Thus the [Second Chern number](../../../../../second-chern-number.md) measures the obstruction to choosing one trivialization over the whole four-sphere.

A simpler [First Chern class](../../../../../first-chern-class.md) example is a line bundle over $S^2$. Write $A=-ia$ and choose local real potentials

$$
a_N=\frac{k}{2}(1-\cos\theta)d\phi,\qquad
a_S=-\frac{k}{2}(1+\cos\theta)d\phi.
$$

They have common curvature $da=(k/2)\sin\theta\,d\theta\wedge d\phi$, so $\int_{S^2}c_1=(2\pi)^{-1}\int da=k$. Their difference $a_N-a_S=k\,d\phi$ corresponds to the transition function $e^{-ik\phi}$, which is single-valued exactly when $k\in\mathbb Z$. This illustrates how the global integer arises from patching, rather than from an arbitrary flux normalization.

In physics, these constructions distinguish topological sectors of [Yang-Mills instantons](../../../../../yang-mills-instanton.md) and relate four-dimensional characteristic densities to three-dimensional boundary actions. The [Chern-Simons three-form](../../../../../chern-simons-3-form.md) itself gives a metric-independent gauge action in three dimensions. On a closed manifold its first variation is

$$
\delta\int Y=\frac1{4\pi^2}\int\operatorname{Tr}(\delta A\wedge F),
$$

so its classical equation is **$F=0$**. The common thread is that a local expression in the [connection one-form](../../../../../connection-one-form.md) records global topology: curvature produces the invariant [Chern number](../../../../../chern-number.md), while its local [Chern-Simons three-form](../../../../../chern-simons-3-form.md) primitive retains gauge and boundary information.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
