<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [congruence on a category](../../../../../congruence-on-a-category.md) is an equivalence relation on every hom-set such that $f\sim f'$ and $g\sim g'$ imply $gf\sim g'f'$ whenever the composites exist. The quotient has the same objects and equivalence classes $[f]$ as morphisms.

For the proposed $\Phi$-maps, reflexivity uses $W=U$, symmetry is immediate, and transitivity is obtained as follows. If representatives over $U$ and $V$ agree after restriction to $W$, while those over $V$ and $T$ agree after restriction to $W'$, then their first and third representatives agree over $W\times W'$. This object belongs to $\Phi$ and maps below $U\times T$, proving transitivity.

The identity of $A$ is represented by the projection $A\times1\to A$. If $f:A\times U\to B$ and $g:B\times V\to C$, define their composite over $U\times V$ by

$$
A\times U\times V\xrightarrow{f\times1_V}B\times V\xrightarrow{g}C.
$$

Passing to a smaller member of $\Phi$ shows that this is independent of representatives. Associativity follows from associativity of products and composition, and the projection representatives satisfy the identity laws. This constructs the [category of partial maps localized at subterminal objects](../../../../../category-of-partial-maps-localized-at-subterminal-objects.md) $\mathcal C_\Phi$.

The terminal object remains $1$. Products are the products of $\mathcal C$: representatives $f:C\times U\to A$ and $g:C\times V\to B$ pair after restriction to $U\times V$,

$$
C\times U\times V\longrightarrow A\times B.
$$

The product universal property follows after restricting competing representatives to a common member of $\Phi$. The functor $P_\Phi$ sends the original projections and pairings to these, so it preserves finite products.

If $\mathcal C$ is [Cartesian closed](../../../../../cartesian-closed-category.md), use the same exponential object $B^A$. A representative

$$
f:(C\times A)\times U\to B
$$

may be rearranged as $(C\times U)\times A\to B$ and curried in $\mathcal C$ to $C\times U\to B^A$. Currying respects restriction and gives a natural bijection

$$
\mathcal C_\Phi(C\times A,B)\cong\mathcal C_\Phi(C,B^A).
$$

Thus $\mathcal C_\Phi$ is cartesian closed and $P_\Phi$ preserves exponentials.

In general this is not a quotient by a congruence. A congruence can identify existing parallel morphisms but cannot create a morphism between two objects. Take $\mathcal C=\mathbf{Set}$ and $\Phi=\{0,1\}$, the filter containing the empty subobject of the terminal set. Then every $A\times0\to B$ represents a $\Phi$-map, so in particular $\mathcal C_\Phi(A,\varnothing)$ is nonempty for nonempty $A$, whereas $\mathbf{Set}(A,\varnothing)$ is empty. Hence no quotient of $\mathbf{Set}$ by a congruence is isomorphic to this $\mathcal C_\Phi$ by an identity-on-objects functor.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
