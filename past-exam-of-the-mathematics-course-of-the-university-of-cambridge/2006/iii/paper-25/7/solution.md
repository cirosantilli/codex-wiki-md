<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For nonempty [first-order structures](../../../../../first-order-structure.md) $(M_i)_{i\in I}$ in a common language and an [ultrafilter](../../../../../ultrafilter.md) $D$ on $I$, identify product [functions](../../../../../function-split.md) by

$$
f\sim_D g\quad\Longleftrightarrow\quad\{i:f(i)=g(i)\}\in D.
$$

The [ultraproduct](../../../../../ultraproduct.md) $\prod_i M_i/D$ has these equivalence classes as elements. [Functions](../../../../../function-split.md) are interpreted coordinatewise, and a relation holds of classes exactly when its coordinatewise truth [set](../../../../../set-split.md) belongs to $D$. Closure under finite [intersections](../../../../../set-intersection.md) makes these interpretations independent of representatives.

The [Łoś theorem](../../../../../los-theorem.md) asserts

$$
\prod_i M_i/D\models\varphi([f_1],\ldots,[f_n])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(f_1(i),\ldots,f_n(i))\}\in D.
$$

Prove it by induction on [first-order formulas](../../../../../first-order-formula.md). Atomic [first-order formulas](../../../../../first-order-formula.md) hold by the definitions and induction on terms. Conjunction uses [intersections](../../../../../set-intersection.md), and negation uses the fact that an [ultrafilter](../../../../../ultrafilter.md) contains exactly one of a [set](../../../../../set-split.md) and its complement. For an existential [first-order formula](../../../../../first-order-formula.md), a product witness gives a coordinate witness on a $D$-large [set](../../../../../set-split.md). Conversely, on the $D$-large [set](../../../../../set-split.md) where a coordinate witness exists, choose one in each factor, and choose arbitrary values elsewhere. Its class is a product witness by the induction hypothesis. This is the only witness-selection step; the surrounding argument is made in a choice metatheory. The special case with all factors equal is an [ultrapower](../../../../../ultrapower.md), and constant [functions](../../../../../function-split.md) give an [elementary embedding](../../../../../elementary-embedding.md).

Here is a direct [compactness theorem](../../../../../compactness-theorem.md) proof. Suppose every finite [subset](../../../../../subset.md) of a theory $T$ has a model. Index factors by the finite [subsets](../../../../../subset.md) $i\subseteq T$, choosing $M_i\models i$. For finite $F\subseteq T$, the cone $C_F=\{i:F\subseteq i\}$ is nonempty, and $C_F\cap C_H=C_{F\cup H}$. Extend the generated proper filter to an [ultrafilter](../../../../../ultrafilter.md) $D$. For every sentence $\sigma\in T$, its truth [set](../../../../../set-split.md) contains $C_{\{\sigma\}}$, so the [Łoś theorem](../../../../../los-theorem.md) gives $\prod_iM_i/D\models T$. **Finite satisfiability therefore implies satisfiability**, directly from the [ultraproduct](../../../../../ultraproduct.md) construction rather than from a syntactic completeness argument.

For [saturated models](../../../../../saturated-model.md), a structure is $\kappa$-saturated if every [complete type](../../../../../complete-type.md) over fewer than $\kappa$ parameters is realized. A useful concrete case is [countable saturation of a nonprincipal ultraproduct over omega](../../../../../countable-saturation-of-a-nonprincipal-ultraproduct-over-omega.md). In a [countable](../../../../../countable-set.md) language, enumerate any finitely satisfiable type over countably many parameters as $\varphi_1(x),\varphi_2(x),\ldots$, and represent its parameters by product [functions](../../../../../function-split.md). By the [Łoś theorem](../../../../../los-theorem.md), the [set](../../../../../set-split.md) $A_n$ of coordinates where the first $n$ [first-order formulas](../../../../../first-order-formula.md) have a simultaneous witness belongs to the [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $D$. Put

$$
B_n=\{i:i\ge n\}\cap\bigcap_{j\le n}A_j.
$$

These are decreasing $D$-large [sets](../../../../../set-split.md). At coordinate $i$, let $h(i)$ be the largest $n\le i$ with $i\in B_n$, or zero if none exists, and choose a witness for the first $h(i)$ [first-order formulas](../../../../../first-order-formula.md). For fixed $n$, every coordinate in $B_n$ has $h(i)\ge n$, so the resulting product [function](../../../../../function-split.md) satisfies $\varphi_n$ on a $D$-large [set](../../../../../set-split.md). Its class realizes the whole type. Thus such an [ultraproduct](../../../../../ultraproduct.md) is $\aleph_1$-saturated.

There is also an existence construction at every prescribed degree $\kappa$. Given an infinite model $M$, choose a [regular cardinal](../../../../../regular-cardinal.md) $\lambda\ge\kappa$ and construct an elementary chain $(M_\alpha)_{\alpha\le\lambda}$. At a successor stage, add a new constant for a realization of every type over every [subset](../../../../../subset.md) of $M_\alpha$ of size below $\kappa$, together with the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md) of $M_\alpha$. Every finite part is satisfiable: only finitely many types and finitely many [first-order formulas](../../../../../first-order-formula.md) from each are involved, and each finite type fragment has a witness in $M_\alpha$. Compactness therefore supplies a simultaneous [elementary extension](../../../../../elementary-extension.md). At limits take [unions](../../../../../set-union.md). To justify elementarity of a [union](../../../../../set-union.md), any existential [first-order formula](../../../../../first-order-formula.md) with parameters in an earlier stage has a witness in that stage whenever it has one at a later stage, by elementarity; this is the [Tarski-Vaught test](../../../../../tarski-vaught-test.md).

Any fewer-than-$\kappa$ parameters of $M_\lambda$ occur together in some $M_\alpha$, by regularity of $\lambda$. A type over them which is finitely satisfiable in $M_\lambda$ is finitely satisfiable in $M_\alpha$, again by elementarity, and was realized in $M_{\alpha+1}$. Hence **every infinite structure has a $\kappa$-saturated [elementary extension](../../../../../elementary-extension.md) for any prescribed cardinal $\kappa$.** No bound on the size of this extension is asserted; full saturation at the model's own [cardinality](../../../../../cardinality.md) has additional cardinal-arithmetic issues.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
