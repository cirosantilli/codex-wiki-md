<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For nonempty [first-order structures](../../../../../../first-order-structure.md) $(M_i)_{i\in I}$ and an [ultrafilter](../../../../../../ultrafilter.md) $\mathcal U$ on $I$, define the [ultraproduct](../../../../../../ultraproduct.md) by quotienting the product domain by

$$
a\sim b\quad\Longleftrightarrow\quad\{i:a_i=b_i\}\in\mathcal U.
$$

Functions are interpreted coordinatewise; a relation holds when its coordinate truth [set](../../../../../../set-split.md) belongs to the [ultrafilter](../../../../../../ultrafilter.md). Closure under finite intersections makes these interpretations independent of representatives. The [Łoś theorem](../../../../../../los-theorem.md) asserts, for every formula $\varphi$,

$$
\boxed{\prod_iM_i/\mathcal U\models\varphi([a^1],\ldots,[a^r])
\Longleftrightarrow
\{i:M_i\models\varphi(a_i^1,\ldots,a_i^r)\}\in\mathcal U.}
$$

Prove it by structural induction. A term evaluates coordinatewise, by induction on its construction, so atomic equality and relations are exactly their defining truth [sets](../../../../../../set-split.md). Conjunction uses intersection; negation uses the [ultrafilter](../../../../../../ultrafilter.md) property that exactly one of a [set](../../../../../../set-split.md) and its complement belongs to $\mathcal U$. These establish all Boolean connectives.

For the existential step put $A=\{i:M_i\models\exists x\,\psi(x,\bar a_i)\}$. If an [ultraproduct](../../../../../../ultraproduct.md) witness $[b]$ exists, induction says $\{i:M_i\models\psi(b_i,\bar a_i)\}\in\mathcal U$, and this [set](../../../../../../set-split.md) is contained in $A$, so $A\in\mathcal U$. Conversely if $A\in\mathcal U$, choose a witness $b_i$ at every $i\in A$ and any domain element at the other coordinates. Induction makes $[b]$ a witness. This coordinatewise selection uses choice in the metatheory; nonemptiness of the factors is essential. Universal quantification follows from negation and existence, completing the proof.

For the requested [compactness theorem](../../../../../../compactness-theorem.md), let $I=[T]^{<\omega}$. For each finite $F\subseteq T$, choose $M_F\models F$. For each sentence $\sigma\in T$, its cone $C_\sigma=\{F:\sigma\in F\}$ is nonempty, and intersections of finitely many cones contain the finite union of their requirements. These cones generate a proper filter. The [ultrafilter lemma](../../../../../../ultrafilter-lemma.md) extends it to $\mathcal U$. The coordinate models satisfying $\sigma$ include $C_\sigma$, so the Łoś theorem makes their [ultraproduct](../../../../../../ultraproduct.md) satisfy $\sigma$. Since this holds for each $\sigma\in T$, **the [ultraproduct](../../../../../../ultraproduct.md) is a model of $T$**. No completeness theorem is needed in this second compactness proof.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
