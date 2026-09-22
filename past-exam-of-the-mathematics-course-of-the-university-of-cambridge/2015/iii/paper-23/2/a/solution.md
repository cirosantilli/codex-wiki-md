<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here is the [existential common-substructure test for quantifier elimination](../../../../../../existential-common-substructure-test-for-quantifier-elimination.md). Use a [first-order language](../../../../../../first-order-language.md) with a constant symbol, as in the applications below, or the usual conventions for empty generated substructures and truth constants. Let $T$ be a [first-order theory](../../../../../../first-order-theory.md). Suppose that whenever $\mathcal M,\mathcal N\models T$ have a common [substructure](../../../../../../substructure-of-a-first-order-structure.md) $\mathcal A$, then, for every [quantifier-free formula](../../../../../../quantifier-free-formula.md) $\theta(x,\bar y)$ and every finite tuple $\bar a\in A$,

$$
\mathcal M\models\exists x\,\theta(x,\bar a)
\quad\Longrightarrow\quad
\mathcal N\models\exists x\,\theta(x,\bar a).
$$

The condition is symmetric because it applies also with $\mathcal M$ and $\mathcal N$ exchanged. The conclusion is **[quantifier elimination](../../../../../../quantifier-elimination.md) for $T$**: for every [first-order formula](../../../../../../first-order-formula.md) $\varphi(\bar y)$ there is a [quantifier-free formula](../../../../../../quantifier-free-formula.md) $\psi(\bar y)$ such that

$$
T\models\forall\bar y\bigl(\varphi(\bar y)\leftrightarrow\psi(\bar y)\bigr).
$$

The common [substructure](../../../../../../substructure-of-a-first-order-structure.md) need not itself satisfy $T$, and witnesses are sought in the whole models, not necessarily in $A$. This test is the [QET1](../../../../../../existential-common-substructure-test-for-quantifier-elimination.md) version of the [common-substructure test for quantifier elimination](../../../../../../common-substructure-test-for-quantifier-elimination.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
