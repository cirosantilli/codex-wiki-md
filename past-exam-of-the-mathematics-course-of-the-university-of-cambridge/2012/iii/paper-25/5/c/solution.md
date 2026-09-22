<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [weakly initial set](../../../../../../weakly-initial-set.md) is a set of objects $(W_i)_{i\in I}$ such that every object receives at least one map from some $W_i$. An [initial object](../../../../../../initial-object.md) is itself a singleton [weakly initial set](../../../../../../weakly-initial-set.md). We prove the converse without replacing uniqueness by weak initiality.

Let $\mathcal E$ be a [complete category](../../../../../../complete-category.md) that is [locally small](../../../../../../locally-small-category.md). Form $W=\prod_i W_i$. For every object $A$, choose $W_i\to A$ and compose with the projection $W\to W_i$, so $W$ is weakly initial. Completeness supplies a [terminal object](../../../../../../terminal-object.md), so the given [weakly initial set](../../../../../../weakly-initial-set.md) cannot be empty.

The [endomorphisms](../../../../../../endomorphism.md) of $W$ form a [set](../../../../../../set-split.md). Take a simultaneous [equalizer](../../../../../../equaliser.md) $e:I\to W$ of all of them with $1_W$; equivalently, equalize the two maps from $W$ into $\prod_{s\in\mathcal E(W,W)}W$ with components $s$ and $1_W$. Thus $se=e$ for every endomorphism $s$. The object $I$ is weakly initial, since $I\xrightarrow eW\to A$ exists for every $A$. Weak initiality of $W$ gives a map $u:W\to I$. Applying the equalizing identity to $eu$ yields $eue=e$, so monicity of $e$ gives $ue=1_I$.

For any [endomorphism](../../../../../../endomorphism.md) $v:I\to I$, the map $evu$ is an [endomorphism](../../../../../../endomorphism.md) of $W$. Therefore $evue=e$. Since $ue=1_I$, this becomes $ev=e$, giving $v=1_I$. Now let $f,g:I\rightrightarrows A$ and form their [equalizer](../../../../../../equaliser.md) $j:E\to I$. Weak initiality of $I$ gives $h:I\to E$. The composite $jh$ is an [endomorphism](../../../../../../endomorphism.md) of $I$, hence the identity. Consequently $f=fjh=gjh=g$.

There is at least one map from $I$ to every object, and the argument proves that there is at most one. **The object $I$ is an [initial object](../../../../../../initial-object.md).** This establishes the [initial-object lemma for complete categories with a weakly initial set](../../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md) using only small [products in a category](../../../../../../product-category-theory.md) and [equalizers](../../../../../../equaliser.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
