<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [ultraproduct](../../../../../ultraproduct.md) assembles a family of nonempty [first-order structures](../../../../../first-order-structure.md) $\langle M_i:i\in I\rangle$ in one fixed language, using an [ultrafilter](../../../../../ultrafilter.md) $U$ to specify which coordinate statements hold almost everywhere. Its universe is

$$
\prod_{i\in I}M_i/U,\qquad
f\sim_Ug\ \Longleftrightarrow\ \{i:f(i)=g(i)\}\in U.
$$

Functions are interpreted coordinatewise, and an $r$-ary relation holds on $[f_1],\ldots,[f_r]$ when its coordinate truth set belongs to $U$. Changing representatives changes such a truth set only off a $U$-large set, so these definitions are well defined. A principal [ultrafilter](../../../../../ultrafilter.md) simply recovers its distinguished factor; a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) can produce new elements and structures.

The fundamental result is the [Łoś theorem](../../../../../los-theorem.md):

$$
\prod_iM_i/U\models\varphi([f_1],\ldots,[f_r])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(f_1(i),\ldots,f_r(i))\}\in U.
$$

Prove it by [structural induction](../../../../../structural-induction.md) on [first-order formulas](../../../../../first-order-formula.md). Atomic formulas are the definition. Intersections handle conjunction, while exactly one of a set and its complement belongs to an [ultrafilter](../../../../../ultrafilter.md), handling negation. For the existential step, if the coordinate existential truth set is in $U$, use [choice](../../../../../axiom-of-choice.md) to select witnesses there and arbitrary values elsewhere; their product function is an ultraproduct witness. Conversely a product witness makes the coordinate existential truth set contain a $U$-large set. Other connectives and universal quantification follow.

In an [ultrapower](../../../../../ultrapower.md), all factors are one structure $M$. The diagonal map $a\mapsto[\text{constant }a]$ is an [elementary embedding](../../../../../elementary-embedding.md) by the [Łoś theorem](../../../../../los-theorem.md). For a nonprincipal $U$ on $\omega$, the class of $n\mapsto n$ in an ultrapower of the standard [natural numbers](../../../../../natural-number.md) is larger than every constant natural number, since each tail belongs to $U$. This gives a [nonstandard model of Peano arithmetic](../../../../../non-standard-model-of-arithmetic.md). Similarly, an ultraproduct of finite [fields](../../../../../field.md) $\mathbb F_{p_i}$ with distinct primes tending to infinity has [characteristic zero](../../../../../characteristic-zero.md): for every fixed positive integer $m$, the equation $m1=0$ fails in all sufficiently late factors. An infinite structure can therefore arise from finite factors.

Ultraproducts prove the [compactness theorem](../../../../../compactness-theorem.md). If each finite subset $\Delta$ of a theory $T$ has a model $M_\Delta$, index these models by $[T]^{<\omega}$. The cones $\{\Delta:\varphi\in\Delta\}$ have the [finite intersection property](../../../../../finite-intersection-property.md). Extend their filter to an [ultrafilter](../../../../../ultrafilter.md) using the [ultrafilter lemma](../../../../../ultrafilter-lemma.md). The [Łoś theorem](../../../../../los-theorem.md) makes the resulting ultraproduct satisfy every $\varphi\in T$. This construction also gives elementary extensions realizing prescribed finitely satisfiable types.

A useful stronger property is [countable saturation of an ultraproduct over omega](../../../../../countable-saturation-of-an-ultraproduct-over-omega.md). Let a countable type $\{\varphi_n(x,\bar a_n):n<\omega\}$ be finitely satisfiable in an ultraproduct over a nonprincipal $U$ on $\omega$. Choose coordinate representatives of its parameters. Let $E_n$ be the coordinates where the first $n$ formulas have a simultaneous witness; then $E_n\in U$, the $E_n$ decrease, and we can replace $E_n$ by $E_n\cap[n,\infty)$. At coordinate $i$, choose a witness to the first $m(i)$ formulas, where $m(i)$ is the largest $n\le i$ with $i\in E_n$, taking an arbitrary value if there is none. For each fixed $n$, the set where $m(i)\ge n$ is $U$-large. Its class realizes the entire type. This proof uses countable incompleteness of $U$, not arbitrary completeness or automatic saturation at larger cardinals.

Finally, complete [ultrafilters](../../../../../ultrafilter.md) connect ultraproducts to large [cardinals](../../../../../cardinal-number.md). A countably complete [ultrafilter](../../../../../ultrafilter.md) prevents an externally infinite descending membership chain in an ultrapower of a well-founded universe: intersect the countably many coordinate truth sets and obtain an impossible descending chain at one coordinate. A [kappa-complete](../../../../../kappa-complete-filter.md) nonprincipal [ultrafilter](../../../../../ultrafilter.md) on $\kappa$ consequently supplies the [ultrapower embedding](../../../../../ultrapower-embedding.md) associated with a [measurable cardinal](../../../../../measurable-cardinal.md). Thus the same construction supports both elementary compactness arguments and large-cardinal embeddings, with the completeness hypothesis deciding which well-foundedness and closure properties survive.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
