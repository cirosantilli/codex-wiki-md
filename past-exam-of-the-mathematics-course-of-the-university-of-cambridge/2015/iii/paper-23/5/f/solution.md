<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the countable-language hypothesis of the [omitting types theorem](../../../../../../omitting-types-theorem.md), which is the usual convention for this prime-model result. Let $\mathcal M$ be a [prime model](../../../../../../prime-model.md) of $T$ and $a\in M$.

First, $T$ is complete up to logical consequence: every model $\mathcal N\models T$ receives an [elementary embedding](../../../../../../elementary-embedding.md) of $\mathcal M$, so it satisfies exactly the same sentences as $\mathcal M$. We may therefore replace $T$ by $\operatorname{Th}(\mathcal M)$ without changing its model class or the [prime model](../../../../../../prime-model.md) property.

Suppose $p=\operatorname{tp}^{\mathcal M}(a/\varnothing)$ were not isolated. The [omitting types theorem](../../../../../../omitting-types-theorem.md), applied to this single [complete type](../../../../../../complete-type.md), would produce $\mathcal N\models T$ omitting $p$. By primality choose an [elementary embedding](../../../../../../elementary-embedding.md) $j:\mathcal M\to\mathcal N$. For every $\varphi(x)\in p$,

$$
\mathcal M\models\varphi(a)\quad\Longrightarrow\quad\mathcal N\models\varphi(j(a)).
$$

Then $j(a)$ realizes $p$, contradicting omission. Consequently

$$
\boxed{\operatorname{tp}^{\mathcal M}(a/\varnothing)\text{ is isolated for every }a\in M.}
$$

The same proof applies to every finite tuple, giving an [atomic model](../../../../../../atomic-model.md). Countability of the language is a hypothesis of this argument, not a restriction on parameter sets in the separate parts (a) and (d). The PDF does not state that standing hypothesis explicitly; it must be included when invoking this version of the theorem.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
