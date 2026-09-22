<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Absolute Frobenius morphism](../../../../../absolute-frobenius-morphism.md) is the identity on the underlying [topological space](../../../../../topological-space.md) and acts on the [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) by $a\mapsto a^p$. On an [affine scheme](../../../../../affine-scheme.md) it is induced by the [ring homomorphism](../../../../../ring-homomorphism.md) $A\to A$, $a\mapsto a^p$. This is additive in characteristic $p$, and the inverse image of a [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$ is again $\mathfrak p$, since $a^p\in\mathfrak p$ exactly when $a\in\mathfrak p$. These affine maps agree under [localization](../../../../../localization-of-a-ring.md) and hence glue.

A [perfect ring of characteristic p](../../../../../perfect-ring-of-characteristic-p.md) is one whose [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) is bijective. Since the [Absolute Frobenius morphism](../../../../../absolute-frobenius-morphism.md) fixes points, its map on the [stalk](../../../../../stalk-of-a-sheaf.md) at $x$ is precisely the [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) of $\mathcal O_{X,x}$. A morphism of sheaves is an [isomorphism](../../../../../isomorphism.md) exactly when it is an [isomorphism](../../../../../isomorphism.md) on all [stalks](../../../../../stalk-of-a-sheaf.md). Therefore

$$
\boxed{F_X\text{ is an isomorphism}\iff \mathcal O_{X,x}\text{ is perfect for every }x.}
$$

In the reverse direction the inverse [sheaf](../../../../../sheaf-mathematics.md) map, together with the identity on points, gives the inverse [morphism of locally ringed spaces](../../../../../morphism-of-locally-ringed-spaces.md). This is perfection in the Frobenius sense, not the unrelated homological use of the word perfect.

For the [function field](../../../../../function-field-of-an-algebraic-variety.md) assertions below, interpret the [normal schemes](../../../../../normal-scheme.md) as integral, as is implicit in writing a single [field](../../../../../field.md) $k(X)$ or $k(Y)$. General [normal schemes](../../../../../normal-scheme.md) need not be irreducible; without this interpretation those [fields](../../../../../field.md) are not defined globally as single [fields](../../../../../field.md). Set $K=k(Y)\subseteq L=k(X)$. For an affine open $V=\operatorname{Spec}A$ in $Y$, finiteness gives $f^{-1}V=\operatorname{Spec}B$, with $A\subseteq B$ finite and both [rings](../../../../../ring.md) normal domains. In fact $B$ is the [integral closure](../../../../../integral-closure.md) of $A$ in $L$: any element of $L$ integral over $A$ is also integral over $B$ and therefore belongs to $B$. This local description yields the two forms of [Frobenius factorization through a finite normal cover](../../../../../frobenius-factorization-through-a-finite-normal-cover.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 89](../../paper-89-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
