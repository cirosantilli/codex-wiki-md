<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Here and throughout, a [filter on a set](../../../../../filter-set-theory.md) is proper: it contains the whole underlying set, excludes the empty set, and is upward closed and closed under finite intersections. An improper filter cannot be extended to a proper [ultrafilter](../../../../../ultrafilter.md).

Order the proper filter extensions of $\mathcal F$ by inclusion. The union of a chain is again a proper [filter on a set](../../../../../filter-set-theory.md): any two members already occur in one member of the chain, where their intersection belongs; the empty set never appears. By [Zorn lemma](../../../../../zorn-s-lemma.md), take a maximal proper extension $\mathcal U$. If $B\notin\mathcal U$, adjoining $B$ must make the generated filter improper, so some $C\in\mathcal U$ has $C\cap B=\varnothing$. Upward closure then gives $B^c\in\mathcal U$. Exactly one of $B,B^c$ belongs to $\mathcal U$, proving the [ultrafilter lemma](../../../../../ultrafilter-lemma.md).

Let $M_i$ be nonempty structures for a common [first-order language](../../../../../first-order-language.md), and let $\mathcal U$ be an [ultrafilter](../../../../../ultrafilter.md) on the index set $I$. In the [ultraproduct](../../../../../ultraproduct.md) $M=\prod_iM_i/\mathcal U$, identify functions $f,g$ when $\{i:f(i)=g(i)\}\in\mathcal U$; interpret function symbols coordinatewise and relations by membership of their coordinate truth sets in $\mathcal U$. The [Łoś theorem](../../../../../los-theorem.md) states, for every [first-order formula](../../../../../first-order-formula.md) $\phi$,

$$
M\models\phi([f_1],\ldots,[f_n])\quad\Longleftrightarrow\quad\{i:M_i\models\phi(f_1(i),\ldots,f_n(i))\}\in\mathcal U.
$$

Changing representatives changes a coordinate truth set only outside a member of $\mathcal U$, so the definitions are well defined.

Prove the theorem by [structural induction](../../../../../structural-induction.md) on formulas. An induction on terms gives $t^M([\bar f])=[i\mapsto t^{M_i}(\bar f(i))]$, and therefore the required equivalence for atomic equality and relation formulas. For conjunction the truth set is an intersection, and a finite intersection belongs to a proper [filter on a set](../../../../../filter-set-theory.md) exactly when each constituent does. For negation it is a complement, and the [ultrafilter](../../../../../ultrafilter.md) decides exactly one of a set and its complement. These prove the Boolean induction steps.

For the existential step, a witness $[g]$ in $M$ gives, by induction, a member of $\mathcal U$ on which $\phi(g(i),\bar f(i))$ holds. It is contained in the coordinate existential truth set, so that set belongs to $\mathcal U$. Conversely, if

$$
J=\{i:M_i\models\exists x\,\phi(x,\bar f(i))\}\in\mathcal U,
$$

choose a coordinate witness $g(i)$ for $i\in J$, and any element of the nonempty factor otherwise. Then the truth set of $\phi(g(i),\bar f(i))$ contains $J$. Induction gives a witness $[g]$ in the [ultraproduct](../../../../../ultraproduct.md). Universal quantification follows from negation and existence. This completes the actual proof of the [Łoś theorem](../../../../../los-theorem.md).

For the [compactness theorem](../../../../../compactness-theorem.md), take $I$ to be the set of finite subsets $\Delta$ of $T$, and choose a model $M_\Delta$ of each such subset. The cones

$$
I_\Gamma=\{\Delta\in I:\Gamma\subseteq\Delta\}\qquad(\Gamma\subseteq T\text{ finite})
$$

are nonempty and satisfy $I_{\Gamma_1}\cap I_{\Gamma_2}=I_{\Gamma_1\cup\Gamma_2}$. They generate a proper [filter on a set](../../../../../filter-set-theory.md), which extends to an [ultrafilter](../../../../../ultrafilter.md) $\mathcal U$ by the proved lemma. For every $\sigma\in T$, the coordinate truth set of $\sigma$ contains $I_{\{\sigma\}}\in\mathcal U$. The [Łoś theorem](../../../../../los-theorem.md) therefore gives

$$
\boxed{\prod_{\Delta\in I}M_\Delta/\mathcal U\models T.}
$$

This proves the requested [compactness theorem](../../../../../compactness-theorem.md). In fact the same proof works without the countability restriction on the language.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
