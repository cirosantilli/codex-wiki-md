<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [model](../../../../../model-of-a-first-order-theory.md) is prime if it has an [elementary embedding](../../../../../elementary-embedding.md) into every [model](../../../../../model-of-a-first-order-theory.md) of $T$. A [model](../../../../../model-of-a-first-order-theory.md) is atomic if every finite tuple realizes an isolated [complete type](../../../../../complete-type.md) over the empty [set](../../../../../set-split.md).

If $A$ is prime, the downward [Löwenheim-Skolem theorem](../../../../../lowenheim-skolem-theorem.md) gives a [countable](../../../../../countable-set.md) [model](../../../../../model-of-a-first-order-theory.md) $M$ of $T$, and an [elementary embedding](../../../../../elementary-embedding.md) $A\to M$ makes $A$ [countable](../../../../../countable-set.md). If a tuple of $A$ realized a nonisolated type, the [omitting types theorem](../../../../../omitting-types-theorem.md) would give a [model](../../../../../model-of-a-first-order-theory.md) of $T$ omitting that type. The prime [embedding](../../../../../structure-embedding.md) into it would preserve the tuple's full type and realize the [omitted type](../../../../../omitted-type.md), a [contradiction](../../../../../contradiction.md). Thus a [prime model](../../../../../prime-model.md) is [countable](../../../../../countable-set.md) and atomic.

Conversely enumerate a [countable](../../../../../countable-set.md) [atomic model](../../../../../atomic-model.md) as $a_0,a_1,\ldots$, and take any $B\models T$. Build finite [partial elementary maps](../../../../../partial-elementary-map.md) into $B$. Suppose the current tuple $\bar a$ maps to $\bar b$. Choose a formula $\theta(\bar x,y)$ isolating the type of $(\bar a,a_n)$. The assertion $\exists y\theta(\bar a,y)$ holds in $A$, so its counterpart holds at $\bar b$ in $B$ by partial elementarity. Choose a witness $b_n$. Since $\theta$ isolates the entire extended tuple type, the extended map is elementary on its finite domain; its equality formulas ensure distinct [Elements](../../../../../euclid-s-elements.md) remain distinct. The [union](../../../../../set-union.md) is a total [elementary embedding](../../../../../elementary-embedding.md) $A\to B$. The empty initial tuple works because $T$ is complete. Hence

$$
\boxed{A\text{ is prime}\quad\Longleftrightarrow\quad A\text{ is countable and atomic}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
