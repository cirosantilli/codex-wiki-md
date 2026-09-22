<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [adjunction](../../../../../adjoint-functors.md) $F\dashv G$ is equivalently specified by a [unit and counit of an adjunction](../../../../../unit-and-counit-of-an-adjunction.md)

$$
\eta:1_{\mathcal C}\to GF,\qquad\varepsilon:FG\to1_{\mathcal D}
$$

satisfying the triangle identities

$$
\varepsilon_F\circ F\eta=1_F,\qquad G\varepsilon\circ\eta_G=1_G.
$$

Let $F_i\dashv G_i$ have units $\eta_i$ and counits $\varepsilon_i$. The [mate correspondence](../../../../../mate-correspondence.md) sends $\alpha:F_1\to F_2$ to

$$
\bar\alpha:
G_2\xrightarrow{\eta_1G_2}G_1F_1G_2
\xrightarrow{G_1\alpha G_2}G_1F_2G_2
\xrightarrow{G_1\varepsilon_2}G_1.
$$

Conversely, $\beta:G_2\to G_1$ gives

$$
F_1\xrightarrow{F_1\eta_2}F_1G_2F_2
\xrightarrow{F_1\beta F_2}F_1G_1F_2
\xrightarrow{\varepsilon_1F_2}F_2.
$$

Naturality and the triangle identities show that the two constructions are inverse, yielding the required bijection of [natural transformations](../../../../../natural-transformation.md).

Now let the endofunctor $F$ carry a [monad](../../../../../monad.md) $(F,\eta,\mu)$ and let $F\dashv G$. Taking right mates turns

$$
\eta:1\to F,\qquad\mu:F^2\to F
$$

into a counit $\epsilon:G\to1$ and comultiplication $\delta:G\to G^2$. Since mates reverse composition, the monad unit and associativity laws become the comonad counit and coassociativity laws. Moreover, a map $FA\to A$ corresponds under the adjunction to a map $A\to GA$, and the algebra axioms correspond exactly to the coalgebra axioms. This is the [monad on a left adjoint induces a comonad on its right adjoint](../../../../../monad-on-a-left-adjoint-induces-a-comonad-on-its-right-adjoint.md) construction and gives an isomorphism of the two structure categories.

For a [monoid](../../../../../monoid.md) $M$, the free-$M$-set functor is $F(X)=M\times X$, and its algebras are precisely left $M$-sets, the objects of $[M,\mathbf{Set}]$. Its right adjoint is $G(X)=X^M$. The preceding isomorphism identifies $[M,\mathbf{Set}]$ with the [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) of coalgebras for the induced comonad on sets, compatibly with the forgetful functor. Therefore

$$
\boxed{[M,\mathbf{Set}]\longrightarrow\mathbf{Set}\text{ is comonadic}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
