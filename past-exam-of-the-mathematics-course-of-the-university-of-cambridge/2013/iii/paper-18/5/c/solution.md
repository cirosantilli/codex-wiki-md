<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [initial object](../../../../../../initial-object.md) by itself is a [weakly initial set](../../../../../../weakly-initial-set.md). For the converse, let $(W_i)_{i\in I}$ be a small weakly initial family and form its [product in a category](../../../../../../product-category-theory.md) $W$. Given $X$, choose an arrow $W_i\to X$; its composite with the projection $W\to W_i$ shows that $W$ is weakly initial.

Local smallness makes $\operatorname{End}(W)$ a [set](../../../../../../set-split.md), so completeness supplies the simultaneous [equalizer](../../../../../../equaliser.md) $e:E\to W$ of all endomorphisms of $W$ with $1_W$. Thus $he=e$ for every $h\in\operatorname{End}(W)$. The object $E$ is weakly initial because it maps to $W$.

For parallel arrows $a,b:E\to X$, take their [equalizer](../../../../../../equaliser.md) $j:Y\to E$. Weak initiality of $W$ supplies $t:W\to Y$. The endomorphism $ejt$ of $W$ satisfies $(ejt)e=e$, and monicity of $e$ gives $jte=1_E$. Therefore $j$ is both a [monomorphism](../../../../../../monomorphism.md) and a [split epimorphism](../../../../../../split-epimorphism.md), hence an [isomorphism](../../../../../../isomorphism.md). Since $aj=bj$, we obtain $a=b$. There is already at least one arrow from $E$ to every $X$, so $E$ is initial. This proves the [initial-object lemma for complete categories with a weakly initial set](../../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md), with smallness used exactly where the endomorphisms are equalized.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
