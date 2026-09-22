<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

An [ultraproduct](../../../../../ultraproduct.md) converts coordinatewise finite information into a single [first-order structure](../../../../../first-order-structure.md). Let $(M_i)_{i\in I}$ be nonempty structures in a common [first-order language](../../../../../first-order-language.md), and let $U$ be an [ultrafilter](../../../../../ultrafilter.md) on $I$. In $\prod_iM_i$, [set](../../../../../set-split.md)

$$
f\sim_U g\quad\Longleftrightarrow\quad\{i:f(i)=g(i)\}\in U.
$$

The [ultraproduct](../../../../../ultraproduct.md) $\prod_iM_i/U$ has these [equivalence classes](../../../../../equivalence-class.md) as its elements. [Functions](../../../../../function-split.md) are interpreted coordinatewise; a relation holds of classes exactly when it holds on a $U$-large [set](../../../../../set-split.md) of indices. Intersecting finitely many large agreement [sets](../../../../../set-split.md) shows that these interpretations are independent of representatives.

The [Łoś theorem](../../../../../los-theorem.md), which explains the construction's usefulness, says

$$
\prod_iM_i/U\models\varphi([f_1],\ldots,[f_r])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(f_1(i),\ldots,f_r(i))\}\in U.
$$

Here is the proof. Induction on terms establishes the coordinatewise interpretation of atomic formulas. Finite intersections handle conjunction, and the [ultrafilter](../../../../../ultrafilter.md) property handles negation, since precisely one of a [set](../../../../../set-split.md) and its complement is large. For an [existential quantification](../../../../../existential-quantification.md), a witness class gives coordinate witnesses on a large [set](../../../../../set-split.md). Conversely, when the coordinate existential truth [set](../../../../../set-split.md) is large, select a witness in each of those structures and a default element elsewhere. Its class is a witness in the [ultraproduct](../../../../../ultraproduct.md). This uses [choice](../../../../../axiom-of-choice.md). Structural induction on formulas now proves the theorem, with universal quantification obtained by negation.

**Compactness.** If every finite [subset](../../../../../subset.md) of a first-order theory $T$ has a model, take $I$ to be the finite [subsets](../../../../../subset.md) $\Gamma\subseteq T$ and choose $M_\Gamma\models\Gamma$. The cones $\{\Gamma:\Delta\subseteq\Gamma\}$ for finite $\Delta$ have the finite intersection property. Extend their filter to an [ultrafilter](../../../../../ultrafilter.md) by the [ultrafilter lemma](../../../../../ultrafilter-lemma.md). For each $\varphi\in T$, its cone is large, so the Łoś theorem makes the [ultraproduct](../../../../../ultraproduct.md) satisfy $\varphi$. This proves the [compactness theorem](../../../../../compactness-theorem.md), including theories of arbitrary [set](../../../../../set-split.md) size.

**Elementary extensions and nonstandard elements.** An [ultrapower](../../../../../ultrapower.md) uses a fixed structure at every coordinate. The diagonal map sending $a$ to the class of the constant [function](../../../../../function-split.md) $a$ is an [elementary embedding](../../../../../elementary-embedding.md) by the Łoś theorem. For a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) on $\omega$, the class of $i\mapsto i$ in an [ultrapower](../../../../../ultrapower.md) of the natural numbers exceeds every standard integer, because each corresponding tail is large. In an [ultrapower](../../../../../ultrapower.md) of the real ordered field, the reciprocal of this element is positive and smaller than every positive standard reciprocal integer: an infinitesimal. These examples implement ordinary finite statements in a larger structure without claiming that every external [subset](../../../../../subset.md) or second-order assertion transfers.

**Saturation.** Such an [ultraproduct](../../../../../ultraproduct.md) over $\omega$ is countably saturated. To see the actual diagonal argument, list a finitely satisfiable type $\varphi_0(x),\varphi_1(x),\ldots$ with parameters in the [ultraproduct](../../../../../ultraproduct.md) and fix representatives for those parameters. For each $n$, the [set](../../../../../set-split.md) $E_n$ of coordinates admitting a simultaneous witness to its first $n$ formulas belongs to $U$ by the Łoś theorem. Arrange that the $E_n$ decrease and put $D_n=E_n\cap\{i:i\geq n\}$. The $D_n$ decrease, belong to $U$, and have empty intersection. At coordinate $i$, choose a witness to the first $m(i)$ formulas, where $m(i)$ is the largest $n$ with $i\in D_n$, or choose a default element if there is no such $n$. For each fixed $n$, $m(i)\geq n$ on the large [set](../../../../../set-split.md) $D_n$. Therefore the resulting class realizes every formula. This proves [countable saturation of an ultraproduct over omega](../../../../../countable-saturation-of-an-ultraproduct-over-omega.md); it does not assert saturation at all larger cardinalities.

**Algebraic limits.** Take finite fields $\mathbb F_p$ indexed by the primes and a nonprincipal [ultrafilter](../../../../../ultrafilter.md). Their [ultraproduct](../../../../../ultraproduct.md) is a field of characteristic zero: for every fixed positive integer $n$, only finitely many primes divide $n$, so $n\cdot1\ne0$ on a large [set](../../../../../set-split.md). Every first-order sentence true in all finite fields holds in this infinite field, and more generally so does any sentence true for all but finitely many of the factors. This is a way to create an infinite field retaining uniform first-order information from finite fields. It does not make the field algebraically [closed](../../../../../closed-set.md): the first-order sentence that every element is a square already fails in infinitely many of the factors.

**Large [cardinals](../../../../../cardinal-number.md).** A [countably complete ultrafilter](../../../../../countably-complete-ultrafilter.md) gives a well-founded membership [ultrapower](../../../../../ultrapower.md) of the universe. If it had an infinite descending chain represented by $f_n$, each [set](../../../../../set-split.md)

$$
A_n=\{i:f_{n+1}(i)\in f_n(i)\}
$$

would be large. [Countable](../../../../../countable-set.md) completeness makes $\bigcap_nA_n$ nonempty, giving an actual infinite membership descent at any index in the intersection, contrary to [foundation](../../../../../axiom-of-regularity.md). The [Mostowski collapse](../../../../../mostowski-collapse.md) therefore gives a transitive target and an [ultrapower embedding](../../../../../ultrapower-embedding.md) $j:V\to M$.

For a measure on a [measurable cardinal](../../../../../measurable-cardinal.md) $\kappa$, every [function](../../../../../function-split.md) $\kappa\to\alpha$ with $\alpha<\kappa$ is constant on a large [set](../../../../../set-split.md): otherwise intersect the fewer than $\kappa$ complements of all its fibres. Consequently $j$ fixes the [ordinals](../../../../../ordinal.md) below $\kappa$. The class of the identity [function](../../../../../function-split.md) is below $j(\kappa)$ and above every constant class below $\kappa$, since all tails are large. Thus $j(\kappa)>\kappa$ and its [critical point](../../../../../critical-point.md) is $\kappa$. [Fine ultrafilters](../../../../../fine-ultrafilter.md) on $P_\kappa(\lambda)$ that are [normal ultrafilters on small subsets](../../../../../normal-ultrafilter-on-small-subsets.md) and [kappa-complete](../../../../../kappa-complete-filter.md) yield the stronger embeddings witnessing [supercompact cardinals](../../../../../supercompact-cardinal.md).

These applications share a single principle: **an [ultraproduct](../../../../../ultraproduct.md) preserves precisely the first-order information seen by its [ultrafilter](../../../../../ultrafilter.md)**. Principal [ultrafilters](../../../../../ultrafilter.md) merely select a factor; nonprincipal ones can produce new sizes, elements and saturation. Existence of the needed [ultrafilters](../../../../../ultrafilter.md) and selection of coordinate witnesses are set-theoretic assumptions, and changing the [ultrafilter](../../../../../ultrafilter.md) may change the resulting model.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
