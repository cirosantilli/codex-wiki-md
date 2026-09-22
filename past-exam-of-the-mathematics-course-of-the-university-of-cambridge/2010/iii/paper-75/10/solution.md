<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Let $\mathbf{FinPos}$ be a small skeleton of finite [partially ordered sets](../../../../../partially-ordered-set.md) with all weak [order-preserving functions](../../../../../order-preserving-function.md), and let $\mathbf{FinSPos}$ consist of finite [strict partial orders](../../../../../strict-partial-order.md) with all [strict order-preserving functions](../../../../../strict-order-preserving-function.md). Include the empty structure, because no inhabitation axiom has been imposed. The two classifiers are

$$
\boxed{\mathcal E_1\simeq[\mathbf{FinPos},\mathbf{Set}],\qquad
\mathcal E_2\simeq[\mathbf{FinSPos},\mathbf{Set}]}.
$$

These are covariant functor categories, or presheaves on the opposite finite-model categories; reversing this variance would give the wrong generic models. In each case the generic carrier sends a finite model to its underlying set, with the generic relation given by its order at that stage. These are the [classifying topos of partial orders](../../../../../classifying-topos-of-partial-orders.md) and the [classifying topos of strict partial orders](../../../../../classifying-topos-of-strict-partial-orders.md).

We justify the finite-model presentations internally, so an identification of set-based model categories alone is not being mistaken for a classifying property. A finite weak-order presentation takes a finite graph of required inequalities, closes it transitively and reflexively, and identifies vertices in mutually reachable cycles; this produces a finite poset representing that positive diagram. For the strict theory, a transitive cycle makes the presentation contradictory by irreflexivity; otherwise transitive closure produces a finite strict poset. Homomorphisms from these presentations into any model are exactly the tuples satisfying the specified finite relations.

More explicitly, an internal model $M$ gives $F_M(P)=\operatorname{Hom}(P,M)$ on the opposite finite-model category. Its finite realizations form an internally filtered system. It is nonempty through the empty presentation. Two realizations combine through a disjoint-union presentation. To equalize parallel presentation maps whose composites in $M$ agree, quotient their target by the finitely many required identifications and close the relation transitively. In the weak case, collapse the resulting mutually comparable blocks; antisymmetry in $M$ guarantees that the realization factors through this quotient. In the strict case, either the quotient is a finite strict poset and gives the required factorization, or it has a cycle, making the supposed realization impossible. These constructions prove the flatness conditions without deciding equality of arbitrary elements of $M$.

Conversely a flat functor gives an internal filtered colimit of finite models with the indicated carrier and relation. Each finite axiom remains true under that filtered presentation. One-point presentations recover every element; two-point comparison presentations recover every relation; and finite identifications recover equality. These constructions are inverse: a realization of any finite diagram in the colimit factors locally through a finite stage, and two such realizations agreeing in the colimit agree after a further stage. Thus internal models in every Grothendieck topos correspond to flat functors on the opposite finite-model category. The presheaf case of the [Diaconescu equivalence for geometric morphisms](../../../../../diaconescu-equivalence-for-geometric-morphisms.md) gives the displayed classifiers. This direct finite-presentation argument is the relevant safeguard in identifying presheaf classifiers; agreement of set-model categories by itself would not suffice, as emphasized in [Research on theories of presheaf type](https://faculty.uml.edu/tbeke/presheaf.pdf).

The [reflexification of a strict partial order](../../../../../reflexification-of-a-strict-partial-order.md) interprets the weak theory by

$$
\boxed{x\le y\quad\Longleftrightarrow\quad(x<y)\vee(x=y)}.
$$

Reflexivity is supplied by the equality disjunct. For transitivity, distribute over the two disjunctions: a pair of strict comparisons composes by strict transitivity, and any equality substitutes into the other comparison. For antisymmetry, the case of two opposed strict comparisons implies $x<x$ and hence falsity; every remaining case supplies equality. All these are coherent deductions, so the interpretation works in an arbitrary topos rather than only in classical sets.

It gives a functor $V:\mathbf{FinSPos}\to\mathbf{FinPos}$ and hence a geometric morphism

$$
\boxed{g:\mathcal E_2\longrightarrow\mathcal E_1,\qquad g^*P=P\circ V}.
$$

This applies Question 5 to $V^{\rm op}$ on the presheaf indexing categories. Every finite weak poset is the reflexification of its classical strict part, so every target indexing object is in the image. Question 5(ii) therefore makes $g$ surjective. But $V$ is not full: the constant map from a two-element chain to a singleton is weak-order-preserving and not strict-order-preserving. Question 5(iii) consequently proves **the morphism is a surjection, not an injection**. The strict part of a weak order would require an inequality predicate, so the classical equivalence of weak and strict orders on sets does not supply an inverse geometric interpretation.

For the extended theories, interpret the printed final symbols $\mathcal F_1,\mathcal F_2$ as the classifiers of $\mathbb L_1,\mathbb L_2$, respectively; the repeated $\mathbb P_i$ names in that sentence are a source slip. Let $\mathbf{FinLin}$ contain finite [totally ordered sets](../../../../../totally-ordered-set.md) and all weak monotone maps, and let $\mathbf{FinSLin}$ contain finite [strict total orders](../../../../../strict-total-order.md) and increasing injections. Again include the empty order. Then **both linear-order classifiers are presheaf toposes**:

$$
\boxed{\mathcal F_1\simeq[\mathbf{FinLin},\mathbf{Set}],\qquad
\mathcal F_2\simeq[\mathbf{FinSLin},\mathbf{Set}]}.
$$

For the weak-total model, two finite nondecreasing realized tuples can locally be merged into a single nondecreasing tuple: compare their first remaining entries using totality, take an entry known to be no larger than the other, and continue. This finite procedure uses only finite totality disjunctions and permits duplicate values; it does not require decidable equality. To equalize maps between finite chains, collapse the convex intervals forced equal by their realization; antisymmetry guarantees that all values in such intervals agree. These give the flatness conditions for $\operatorname{Hom}(P,M)$, and finite tuples recover the model exactly as above.

For a strict-total model, trichotomy merges two finite increasing tuples, identifying entries when the equality alternative holds. Every strict map out of a finite chain is injective: if two indices differ, their images are strictly comparable and cannot be equal. Consequently parallel increasing injections with the same realized tuple are already equal, supplying the equalization condition. The same reconstruction proves the [classifying topos of strict linear orders](../../../../../classifying-topos-of-strict-linear-orders.md) claim; in the weak case it proves the [classifying topos of linear orders](../../../../../classifying-topos-of-linear-orders.md) claim. In particular the latter proof has not silently replaced weak totality by decidable strict trichotomy.

Finally, reflexification sends a strict-total model to a weak-total one. Indeed pulling back weak totality under the interpretation gives

$$
(x<y)\vee(x=y)\vee(y<x),
$$

exactly the strict trichotomy axiom. Thus the original morphism restricts to the corresponding subtoposes, giving the commutative square

$$
\begin{array}{ccc}\mathcal F_2&\xrightarrow{g_{\rm lin}}&\mathcal F_1\\\downarrow&&\downarrow\\\mathcal E_2&\xrightarrow{g}&\mathcal E_1.\end{array}
$$

The vertical embeddings are induced by the full inclusions of finite chains among finite partial orders, and their images classify precisely the added axioms. On presheaves $g_{\rm lin}^*$ is restriction along $V_{\rm lin}:\mathbf{FinSLin}\to\mathbf{FinLin}$. The same object-surjectivity and two-element-collapse argument show that the restricted morphism is also surjective and not an embedding. The exact pullback of the added totality axiom further identifies the square as the corresponding base change of subtoposes.

## ↑ Ancestors (10)

1. [10](../10.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
