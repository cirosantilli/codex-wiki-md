<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $C$ be the [smooth algebraic curve](../../../../../smooth-algebraic-curve.md). A nonzero regular section of a [line bundle](../../../../../line-bundle.md) has an effective zero divisor, so its [degree of a line bundle](../../../../../degree-of-a-line-bundle.md) is nonnegative. Degrees add under tensor products and change sign on taking the dual. We use genuine [line subbundles](../../../../../line-subbundle.md), so their quotients in $E$ are [locally free](../../../../../locally-free-sheaf.md). Both bounds can be proved constructively.

For the upper bound, take a rational frame of $E^*$ over the [function field](../../../../../function-field-of-an-algebraic-variety.md) of $C$. Its two members are [rational sections](../../../../../rational-section-of-a-sheaf-of-modules.md) with only finitely many poles. Choose an [effective divisor](../../../../../effective-cartier-divisor.md) $D$ large enough to bound the pole orders of both [rational sections](../../../../../rational-section-of-a-sheaf-of-modules.md). They become [global sections](../../../../../global-section.md) of $E^*\otimes\mathcal O_C(D)$ and define a [sheaf](../../../../../sheaf-mathematics.md) map

$$
E\longrightarrow\mathcal O_C(D)\oplus\mathcal O_C(D)
$$

which is an isomorphism at the [generic point](../../../../../generic-point.md). It is therefore [injective](../../../../../injective-function.md) as a [sheaf](../../../../../sheaf-mathematics.md) map: a section in its [kernel](../../../../../kernel-of-a-linear-map.md) would vanish generically in a [locally free sheaf](../../../../../locally-free-sheaf.md), which is a [torsion-free sheaf](../../../../../torsion-free-sheaf.md). For any [line subbundle](../../../../../line-subbundle.md) $L\subset E$, at least one of its two component maps into $\mathcal O_C(D)$ is nonzero. Such a map is a nonzero [global section](../../../../../global-section.md) of $\mathcal O_C(D)\otimes L^{-1}$. Its zero [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) is effective, so

$$
\boxed{\deg L\le\deg D.}
$$

This [upper degree bound for line subbundles on a smooth curve](../../../../../upper-degree-bound-for-line-subbundles-on-a-smooth-curve.md) depends only on a choice made for $E$, and applies to every one of its [line subbundles](../../../../../line-subbundle.md).

For the lower-bound question we will actually construct subbundles $\mathcal O_C(-mp_0)$ for every sufficiently large integer $m$, where $p_0$ is a fixed point. First prove the [globally generated vector bundle](../../../../../globally-generated-vector-bundle.md) property rather than assuming that negative-degree inclusions automatically are subbundles.

Apply the upper-bound argument to the rank-two [vector bundle](../../../../../vector-bundle.md) $F=E^*\otimes K_C$, where $K_C$ is the [canonical bundle](../../../../../canonical-bundle.md). Let $B$ be its upper degree bound. Choose $m$ with $m-1>B$. For any point $p\in C$, a nonzero [global section](../../../../../global-section.md) of $F(-mp_0+p)$ would give a nonzero map

$$
\mathcal O_C(mp_0-p)\longrightarrow F.
$$

Its image can be saturated to a [saturated line subbundle on a smooth curve](../../../../../saturated-line-subbundle-on-a-smooth-curve.md) $M\subset F$. Locally the [local ring of a smooth algebraic curve](../../../../../local-ring-of-a-smooth-algebraic-curve.md) is a [discrete valuation ring](../../../../../discrete-valuation-ring.md): dividing out the common power of a uniformizer makes the image a primitive rank-one summand, and its quotient is free. Thus the saturation is indeed a subbundle. The original map gives a nonzero [global section](../../../../../global-section.md) of $M\otimes\mathcal O_C(-mp_0+p)$ and consequently $\deg M\ge m-1$, contradicting the upper bound. Hence $H^0(F(-mp_0+p))=0$ for every $p$. By [Serre duality](../../../../../serre-duality.md),

$$
H^1(E(mp_0-p))\cong H^0(E^*\otimes K_C(-mp_0+p))^*=0.
$$

The [exact sequence](../../../../../exact-sequence.md)

$$
0\longrightarrow E(mp_0-p)\longrightarrow E(mp_0)
\longrightarrow E(mp_0)|_p\longrightarrow0
$$

and its [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) show that evaluation $H^0(E(mp_0))\to E(mp_0)|_p$ is onto for every $p$. This proves the [global generation of positive twists on a smooth curve](../../../../../global-generation-of-positive-twists-on-a-smooth-curve.md) with one bound on $m$ that works at every point.

Write $W=H^0(E(mp_0))$ and $N=\dim W$. The evaluation map $W\otimes\mathcal O_C\to E(mp_0)$ is [surjective](../../../../../surjective-function.md) with [kernel](../../../../../kernel-of-a-linear-map.md) bundle of rank $N-2$. Consider the incidence subset

$$
Z=\{(p,s)\in C\times W:s(p)=0\}.
$$

It is the total space of this [kernel](../../../../../kernel-of-a-linear-map.md) bundle, so $\dim Z=1+(N-2)=N-1$. Its projection into $W$ is closed because $C$ is proper, and its image has dimension at most $N-1<N$. Choose $s$ outside this proper closed subset. It vanishes nowhere. In a local trivialization at any point, one component of $s$ is a unit, so it can be completed to a basis. Therefore $\mathcal O_C\xrightarrow{s}E(mp_0)$ is a subbundle with a [locally free](../../../../../locally-free-sheaf.md) rank-one quotient. Twisting back gives

$$
\boxed{\mathcal O_C(-mp_0)\subset E,\qquad\deg\mathcal O_C(-mp_0)=-m\longrightarrow-\infty.}
$$

This proves the [unbounded negative degrees of line subbundles](../../../../../unbounded-negative-degrees-of-line-subbundles.md). The nowhere-vanishing construction guarantees a subbundle at every point, including the zeros that might otherwise have occurred in a generic meromorphic inclusion. If the curve has several connected components, apply these constructions on each component and add the degrees; the same upper-bound and no-lower-bound conclusions follow.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
