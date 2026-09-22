<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use the hypothesis for the two target structures when they are models of $T$; the common source is their generated [substructure](../../../../../../substructure-of-a-first-order-structure.md) and need not itself be a model of $T$. If the hypothesis is read as applying to all target structures, it is stronger and the same proof applies.

Suppose tuples $\mathbf b\in B$ and $\mathbf c\in C$, with $B,C\models T$, have the same complete [quantifier-free type](../../../../../../quantifier-free-type.md). The substructures they generate are isomorphic by the map

$$
t^B(\mathbf b)\longmapsto t^C(\mathbf c)
$$

for every term $t$. Equality of the [quantifier-free types](../../../../../../quantifier-free-type.md) makes this map well defined and injective and makes it preserve and reflect all relations. Identify these generated substructures with one common structure. The assumption then implies that $\phi(\mathbf b)$ and $\phi(\mathbf c)$ have the same truth value. Thus the truth of $\phi$ is determined by the tuple's [quantifier-free type](../../../../../../quantifier-free-type.md).

For any realization $\mathbf b$ of $\phi$ in a model of $T$, let $p$ be its complete [quantifier-free type](../../../../../../quantifier-free-type.md). The preceding paragraph makes $T\cup p(\mathbf x)\cup\{\neg\phi(\mathbf x)\}$ inconsistent. By [compactness theorem](../../../../../../compactness-theorem.md), a finite conjunction $\delta_p(\mathbf x)$ of members of $p$ satisfies

$$
T\models\delta_p\longrightarrow\phi.
$$

Choose such a conjunction for every [quantifier-free type](../../../../../../quantifier-free-type.md) realized by a $\phi$-tuple. These conjunctions cover every realization of $\phi$. Another application of [compactness theorem](../../../../../../compactness-theorem.md), to $T$ together with $\phi$ and the negations of all the chosen conjunctions, gives a finite subcover $\delta_1,\ldots,\delta_m$. Therefore

$$
\boxed{T\models\phi(\mathbf x)\longleftrightarrow\bigvee_{j=1}^m\delta_j(\mathbf x).}
$$

The right side is a [quantifier-free formula](../../../../../../quantifier-free-formula.md). If there are no realizations of $\phi$, use the always-false [quantifier-free formula](../../../../../../quantifier-free-formula.md). This proves the [common-substructure test for quantifier elimination](../../../../../../common-substructure-test-for-quantifier-elimination.md) for the given formula; it does not assume that the source structures are models of the theory.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
