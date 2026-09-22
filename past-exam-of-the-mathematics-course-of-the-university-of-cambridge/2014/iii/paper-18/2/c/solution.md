<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [projective object in a category](../../../../../../projective-object.md) is an object $P$ such that, for every [epimorphism](../../../../../../epimorphism.md) $e:X\to Y$ and every $u:P\to Y$, there is $v:P\to X$ with $ev=u$.

Let $P=\coprod_{i\in I}P_i$ be a [coproduct in a category](../../../../../../coproduct.md) of [projective objects in a category](../../../../../../projective-object.md), with injections $\iota_i$. Given $e:X\to Y$ epic and $u:P\to Y$, projectivity supplies $v_i:P_i\to X$ with $ev_i=u\iota_i$. Choose these lifts for the set-indexed family. The [coproduct in a category](../../../../../../coproduct.md) supplies a unique $v:P\to X$ satisfying $v\iota_i=v_i$. Since $ev\iota_i=u\iota_i$ for every $i$, its universal property gives $ev=u$.

Thus **[coproducts of projective objects are projective](../../../../../../coproducts-of-projective-objects-are-projective.md)**. For an empty family, $P$ is the [initial object](../../../../../../initial-object.md), and the lifting assertion follows directly from its unique maps. The family-of-lifts step uses the usual [axiom of choice](../../../../../../axiom-of-choice.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
