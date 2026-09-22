<h1 id="13i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Replace the strict [partial order](../../../../../../partially-ordered-set.md) by its reflexive closure $\leq$. Partially order all partial orders on $X$ extending $\leq$ by inclusion. A chain has an upper bound given by its union: transitivity and antisymmetry each concern finitely many pairs, which all lie in one member of the chain. By [Zorn lemma](../../../../../../zorn-s-lemma.md) there is a maximal extension $R$.

If $a,b$ are incomparable under $R$, define

$$
R'=R\ \cup\ \{(x,y):xRa\ \hbox{and}\ bRy\}.
$$

This adds $aR'b$. It is transitive: composing an old pair with a new one stays in the added set; composing two new pairs would require $bRa$, which is impossible. It is antisymmetric: an added pair and a reverse old pair would again imply $bRa$, and two reverse added pairs would do the same. Thus $R'$ is a larger partial order, contradicting maximality. Therefore $R$ is total, and removing its diagonal gives **a total order extending the original strict order**.

A [well-founded relation](../../../../../../well-founded-relation.md) has a minimal element in every nonempty subset; with the [axiom of choice](../../../../../../axiom-of-choice.md) this is equivalent to having no infinite strictly descending sequence. If an extension is a [well-order](../../../../../../well-order.md), its least element in any nonempty subset is minimal for the original relation, so **the original order must be well-founded**.

However **not every total extension need be a well-order**. Take the empty strict order on $\mathbb N$, which is well-founded. Its extension defined by $x\prec y$ if $x>y$ in the usual order is total and has no least element.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13I](../../13i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
