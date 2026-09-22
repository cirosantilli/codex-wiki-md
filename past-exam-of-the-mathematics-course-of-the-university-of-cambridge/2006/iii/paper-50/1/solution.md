<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $X\in L$, define the [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) by $\operatorname{ad}_X(Y)=[X,Y]$. The [Jacobi identity](../../../../../jacobi-identity.md) gives, for every $Z$,

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]Z
=[X,[Y,Z]]-[Y,[X,Z]]
=[[X,Y],Z]=\operatorname{ad}_{[X,Y]}Z.
$$

Thus $\operatorname{ad}$ preserves brackets and is a [Lie algebra representation](../../../../../lie-algebra-representation.md). Its [Killing form](../../../../../killing-form.md) is

$$
\kappa(X,Y)=\operatorname{Tr}(\operatorname{ad}_X\operatorname{ad}_Y).
$$

Using the representation identity and the [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md),

$$
\begin{aligned}
\kappa([X,Y],Z)
&=\operatorname{Tr}([\operatorname{ad}_X,\operatorname{ad}_Y]\operatorname{ad}_Z)\\
&=\operatorname{Tr}(\operatorname{ad}_X[\operatorname{ad}_Y,\operatorname{ad}_Z])
=\kappa(X,[Y,Z]).
\end{aligned}
$$

The [Killing form](../../../../../killing-form.md) is also symmetric by cyclicity.

In a basis $T_a$, write $[T_a,T_b]=c_{ab}{}^dT_d$. The lowered [structure constants](../../../../../structure-constant.md) satisfy

$$
c_{abc}=\kappa([T_a,T_b],T_c)=\kappa(T_a,[T_b,T_c]).
$$

The first expression is antisymmetric in $a,b$ and the second in $b,c$. These transpositions generate all permutations, so **$c_{abc}$ is totally antisymmetric.**

An [invariant subspace](../../../../../invariant-subspace.md) of $L$ under its [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) is exactly an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md): $[L,I]\subseteq I$. A [simple Lie algebra](../../../../../simple-lie-algebra.md) has no nonzero proper ideal, proving **the adjoint representation is irreducible.**

Put $D_X=d(X)$. The same [trace](../../../../../matrix-trace.md) calculation proves invariance of the [Trace form of a Lie algebra representation](../../../../../trace-form-of-a-lie-algebra-representation.md):

$$
H([X,Y],Z)=\operatorname{Tr}([D_X,D_Y]D_Z)
=\operatorname{Tr}(D_X[D_Y,D_Z])=H(X,[Y,Z]).
$$

Because the $D_X$ are [anti-Hermitian](../../../../../skew-hermitian-matrix.md), $H$ is a real symmetric bilinear form. The [Killing form](../../../../../killing-form.md) of a simple [compact Lie algebra](../../../../../compact-lie-algebra.md) is negative definite. Define a real [linear map](../../../../../linear-map.md) $T$ by $H(X,Y)=\kappa(TX,Y)$. Invariance of both forms implies that $T$ commutes with every $\operatorname{ad}_Z$, while symmetry makes $T$ self-adjoint for the positive [inner product](../../../../../inner-product.md) $-\kappa$. By the [spectral theorem](../../../../../spectral-theorem.md), its real [eigenspaces](../../../../../eigenspace.md) are invariant under the [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md). Irreducibility forces a single [eigenvalue](../../../../../eigenvalue.md), so $T=\mu I$ and $H=\mu\kappa$. This also avoids the extra care needed when applying the complex form of the [Schur lemma](../../../../../schur-s-lemma.md) to a real vector space.

The kernel of $d$ is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). It cannot be all of $L$: a trivial representation of [dimension](../../../../../dimension-vector-space.md) greater than one is reducible. Simplicity therefore makes $d$ faithful. For every nonzero $X$,

$$
H(X,X)=\operatorname{Tr}(D_X^2)
=-\operatorname{Tr}(D_X^\dagger D_X)<0.
$$

Hence the [positive trace index for a compact simple Lie algebra](../../../../../positive-trace-index-for-a-compact-simple-lie-algebra.md) gives

$$
\boxed{H_{ab}=-\mu\delta_{ab},\qquad\mu>0}
$$

in the adapted basis.

For the [cubic trace tensor of a Lie algebra representation](../../../../../cubic-trace-tensor-of-a-lie-algebra-representation.md), the identity

$$
\operatorname{Tr}([D_Y,D_XD_ZD_W])=0
$$

expands to

$$
B([Y,X],Z,W)+B(X,[Y,Z],W)+B(X,Z,[Y,W])=0.
$$

Set $Y=T_d$, $X=T_a$, $Z=T_b$, $W=T_c$. Cyclicity of $B$ converts $B_{\ell bc}$ to $B_{bc\ell}$ and $B_{a\ell c}$ to $B_{ca\ell}$. Thus the [invariance identity for a cubic trace tensor](../../../../../invariance-identity-for-a-cubic-trace-tensor.md) is

$$
\boxed{c_{da}{}^\ell B_{bc\ell}
+c_{db}{}^\ell B_{ca\ell}
+c_{dc}{}^\ell B_{ab\ell}=0.}
$$

For the final contraction, it is important to keep the specified index-raising convention. In the adapted basis write $C_{ab}{}^c=c_{ab}{}^c$. Then $c_{abc}=-C_{ab}{}^c$, while raising the last two indices with $\kappa^{ab}=-\delta^{ab}$ gives $c_a{}^{mn}=-C_{am}{}^n$. Total antisymmetry and the definition of the [Killing form](../../../../../killing-form.md) imply

$$
\sum_{m,n}C_{am}{}^nC_{rm}{}^n=-\kappa_{ar}=\delta_{ar},
\qquad
c_a{}^{mn}c_{mn}{}^r=-\delta_a{}^r.
$$

Only the antisymmetric part of $B$ in $m,n$ contributes, so

$$
\begin{aligned}
c_a{}^{mn}B_{mnb}
&=\frac12c_a{}^{mn}\operatorname{Tr}([d(T_m),d(T_n)]d(T_b))\\
&=\frac12c_a{}^{mn}c_{mn}{}^rH_{rb}
=-\frac12H_{ab}.
\end{aligned}
$$

Consequently the [Killing-normalized contraction of a cubic trace tensor](../../../../../killing-normalized-contraction-of-a-cubic-trace-tensor.md) is

$$
\boxed{c_a{}^{mn}B_{mnb}=+\frac{\mu}{2}\delta_{ab}.}
$$

The negative sign printed in the last requested identity is incompatible with raising indices by the inverse [Killing form](../../../../../killing-form.md). The opposite sign is obtained if one instead defines the lowered structure constants using the positive Euclidean metric, a different convention from the one specified.

For a concrete check, take the two-dimensional representation of $\mathfrak{su}(2)$ with $T_a=-i\sigma_a/(2\sqrt2)$, where the $\sigma_a$ are [Pauli matrices](../../../../../pauli-matrices.md). Then

$$
\kappa_{ab}=-\delta_{ab},\quad
H_{ab}=-\frac14\delta_{ab},\quad
c_a{}^{mn}=-\frac1{\sqrt2}\epsilon_{amn},\quad
B_{mnb}=-\frac1{8\sqrt2}\epsilon_{mnb}.
$$

Their contraction is $+\delta_{ab}/8$, confirming the positive sign with $\mu=1/4$ and providing a counterexample to the printed sign.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
