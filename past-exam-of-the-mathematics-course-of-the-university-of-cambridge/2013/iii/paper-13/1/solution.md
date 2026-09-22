<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [ring homomorphism](../../../../../ring-homomorphism.md) is understood to preserve $1$. Start with $\varphi:A\to B$. Its map on [spectra of rings](../../../../../spectrum-of-a-commutative-ring.md) is

$$
g:\operatorname{Spec}B\longrightarrow\operatorname{Spec}A,
\qquad \mathfrak q\longmapsto\varphi^{-1}(\mathfrak q).
$$

Contraction gives a [prime ideal](../../../../../prime-ideal.md), and $g^{-1}(D(a))=D(\varphi(a))$. Thus $g$ is [continuous](../../../../../continuous-function.md) for the [Zariski topology](../../../../../zariski-topology.md). On each [principal open subscheme](../../../../../principal-open-subscheme.md), the [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) map is the [ring homomorphism](../../../../../ring-homomorphism.md)

$$
A_a\longrightarrow B_{\varphi(a)},\qquad
\frac{b}{a^m}\longmapsto\frac{\varphi(b)}{\varphi(a)^m}.
$$

These maps commute with restrictions, so they define a [sheaf morphism](../../../../../morphism-of-sheaves.md) $\mathcal O_X\to g_*\mathcal O_Y$. At $\mathfrak q$, with $\mathfrak p=\varphi^{-1}(\mathfrak q)$, its [stalk](../../../../../stalk-of-a-sheaf.md) map is $A_{\mathfrak p}\to B_{\mathfrak q}$. The inverse image of the [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak qB_{\mathfrak q}$ is $\mathfrak pA_{\mathfrak p}$, so this is a [local homomorphism](../../../../../local-homomorphism-of-local-rings.md). We have constructed a [morphism of locally ringed spaces](../../../../../morphism-of-locally-ringed-spaces.md).

Conversely, let $(g,g^\#)$ be a [morphism of locally ringed spaces](../../../../../morphism-of-locally-ringed-spaces.md). Its map on [global sections](../../../../../global-section.md) gives $\varphi:A\to B$, using $\Gamma(X,\mathcal O_X)=A$ and $\Gamma(Y,\mathcal O_Y)=B$. Fix $\mathfrak q\in Y$ and put $\mathfrak p=g(\mathfrak q)$. Compatibility with the [stalk](../../../../../stalk-of-a-sheaf.md) maps and the [local homomorphism](../../../../../local-homomorphism-of-local-rings.md) property give

$$
a\in\mathfrak p
\iff a/1\in\mathfrak pA_{\mathfrak p}
\iff g^\#_{\mathfrak q}(a/1)\in\mathfrak qB_{\mathfrak q}
\iff\varphi(a)\in\mathfrak q.
$$

Consequently $\mathfrak p=\varphi^{-1}(\mathfrak q)$, so the underlying map is forced. On $D(a)$, the [sheaf morphism](../../../../../morphism-of-sheaves.md) is forced as well: it extends $\varphi$ and sends $a$ to a [unit](../../../../../unit-in-a-ring.md), hence agrees with the displayed map by the [universal property of localization](../../../../../universal-property-of-localization.md). The [principal open subschemes](../../../../../principal-open-subscheme.md) form a basis, so the entire [sheaf morphism](../../../../../morphism-of-sheaves.md) is determined. Taking [global sections](../../../../../global-section.md) of the construction recovers $\varphi$. **The two constructions are inverse**, proving the [affine-target adjunction for schemes](../../../../../affine-target-adjunction-for-schemes.md) in the affine-source case:

$$
\boxed{\operatorname{Hom}_{\mathrm{LRS}}(\operatorname{Spec}B,\operatorname{Spec}A)
\cong\operatorname{Hom}_{\mathrm{Ring}}(A,B).}
$$

To describe the [real affine plane scheme points](../../../../../real-affine-plane-scheme-points.md), write $R=\mathbb R[t_1,t_2]$. It is a [unique factorization domain](../../../../../unique-factorization-domain.md) of [Krull dimension](../../../../../krull-dimension.md) two. Its points are exactly the following [prime ideals](../../../../../prime-ideal.md):

- $(0)$, the [generic point](../../../../../generic-point.md) of the whole [affine plane](../../../../../affine-plane.md).
- $(P)$ for each nonconstant [irreducible polynomial](../../../../../irreducible-polynomial.md) $P\in R$, taken up to multiplication by a nonzero real constant. These are the height-one points, each the [generic point](../../../../../generic-point.md) of the [integral scheme](../../../../../integral-scheme.md) $V(P)$.
- The [maximal ideals](../../../../../maximal-ideal.md), or [closed points](../../../../../closed-point.md). By the [Zariski lemma](../../../../../zariski-s-lemma.md), their [residue fields](../../../../../residue-field.md) are finite algebraic extensions of $\mathbb R$. Because $\mathbb R$ is a [real closed field](../../../../../real-closed-field.md), those fields are $\mathbb R$ or $\mathbb C$. The first type is $(t_1-a,t_2-b)$ with $(a,b)\in\mathbb R^2$. The second type is the kernel of evaluation $R\to\mathbb C$ at a nonreal pair $(a,b)\in\mathbb C^2\setminus\mathbb R^2$; the pairs $(a,b)$ and $(\bar a,\bar b)$ give the same [maximal ideal](../../../../../maximal-ideal.md), and these are the only repetitions.

For completeness, any height-one [prime ideal](../../../../../prime-ideal.md) contains an [irreducible polynomial](../../../../../irreducible-polynomial.md) $P$; since $(P)$ is already a height-one [prime ideal](../../../../../prime-ideal.md), it must equal $(P)$. Every remaining nonzero [prime ideal](../../../../../prime-ideal.md) has height two and is maximal, by [Krull dimension](../../../../../krull-dimension.md). For a nonreal pair, evaluation generates all of $\mathbb C$ over $\mathbb R$, so its kernel is maximal. Conversely, each [residue field](../../../../../residue-field.md) isomorphic to $\mathbb C$ has exactly the two conjugate real-algebra embeddings into $\mathbb C$, proving the assertion about repetitions.

This describes the topology too: $V(I)$ consists of the [prime ideals](../../../../../prime-ideal.md) containing $I$, and the closure of a point $\mathfrak p$ is $V(\mathfrak p)$. In particular, the closure of $(0)$ is the whole [affine plane](../../../../../affine-plane.md), while the closure of $(P)$ contains precisely the [closed points](../../../../../closed-point.md) on $P=0$, together with $(P)$ itself. **The spectrum is much larger than the set $\mathbb R^2$.** For example, $(t_1^2+1)$ is a height-one point although its curve has no real points. Its [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) has $\mathcal O(D(h))=R_h$ and [stalk](../../../../../stalk-of-a-sheaf.md) $R_{\mathfrak p}$ at $\mathfrak p$.

The induced [morphism of schemes](../../../../../morphism-of-schemes.md)

$$
\pi:\operatorname{Spec}\mathbb C[t_1,t_2]\longrightarrow\operatorname{Spec}R
$$

is contraction of [prime ideals](../../../../../prime-ideal.md), with the [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) maps given above. On [closed points](../../../../../closed-point.md), it sends $(t_1-a,t_2-b)$ to the kernel of real-polynomial evaluation at $(a,b)$. A real [closed point](../../../../../closed-point.md) has one complex point above it; a nonreal [closed point](../../../../../closed-point.md) has two, interchanged by [complex conjugation](../../../../../complex-conjugation.md). The source [generic point](../../../../../generic-point.md) maps to the target [generic point](../../../../../generic-point.md). The source height-one points are generated by irreducible complex polynomials $Q$. Their contractions are height-one [prime ideals](../../../../../prime-ideal.md) $(P)$, and $Q$ is a factor of $P$ over $\mathbb C$. An irreducible real $P$ either stays irreducible over $\mathbb C$ or splits into two distinct conjugate irreducible factors. Indeed, [complex conjugation](../../../../../complex-conjugation.md) acts transitively on its distinct factors, or a proper orbit product would give a real factor of $P$; every orbit has size at most two. Repeated factors are excluded by separability in [characteristic zero](../../../../../characteristic-zero.md). Thus one or two height-one points lie above $(P)$.

The [complexification fibres of a real scheme](../../../../../complexification-fibres-of-a-real-scheme.md) give a uniform description of all [scheme-theoretic fibres](../../../../../scheme-theoretic-fibre.md), including the nonclosed points, is especially useful. The extension of [coordinate rings](../../../../../coordinate-ring.md) is

$$
\mathbb C[t_1,t_2]\cong R[s]/(s^2+1),
$$

a free $R$-[module](../../../../../module-mathematics.md) with basis $1,s$. At $\mathfrak p\in\operatorname{Spec}R$, with [residue field](../../../../../residue-field.md) $K=\kappa(\mathfrak p)$, the [scheme-theoretic fibre](../../../../../scheme-theoretic-fibre.md) is

$$
\boxed{\pi^{-1}(\mathfrak p)_{\mathrm{sch}}
=\operatorname{Spec}\bigl(K[s]/(s^2+1)\bigr).}
$$

If $-1$ is a square in $K$, the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives $K\times K$, hence two points. Otherwise it is a quadratic [field extension](../../../../../field-extension.md), hence one point. The polynomial has no repeated root in [characteristic zero](../../../../../characteristic-zero.md), so all these [scheme-theoretic fibres](../../../../../scheme-theoretic-fibre.md) are [reduced schemes](../../../../../reduced-scheme.md). This also proves surjectivity. Conjugation acts on each two-point fibre by exchanging its points and fixes each one-point fibre. As a [finite morphism](../../../../../finite-morphism.md), $\pi$ is closed, so its underlying topological space is the quotient by [complex conjugation](../../../../../complex-conjugation.md). The fibre formula explains why a real closed point gives one complex point, whereas the generic point gives a single point with [residue field](../../../../../residue-field.md) $\mathbb C(t_1,t_2)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
