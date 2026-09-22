<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $M$ is a [prime model](../../../../../../prime-model.md). By the downward Lowenheim-Skolem theorem, $T$ has a countable model, and the elementary embedding of $M$ into it makes $M$ countable. If a tuple $\bar a\in M$ had a nonisolated type, the omitting types theorem would give a countable model of $T$ omitting that type. An elementary embedding of $M$ into this model would realize it, a contradiction. Thus $M$ is [atomic](../../../../../../atomic-model.md).

Conversely, let $M$ be countable and atomic, enumerate it as $(a_i)_{i<\omega}$, and let $N\models T$. Construct an elementary embedding recursively. Suppose $a_0,\ldots,a_{n-1}$ have been mapped to $\bar b$. Let $\psi(\bar x)$ isolate the type of $(a_0,\ldots,a_{n-1})$ and let $\theta(\bar x,y)$ isolate the type of $(a_0,\ldots,a_n)$. Since the latter extends the former and is realized in $M$, completeness gives

$$
T\models\forall\bar x\,
\bigl(\psi(\bar x)\to\exists y\,\theta(\bar x,y)\bigr).
$$

The tuple $\bar b$ realizes $\psi$, so a suitable image of $a_n$ exists in $N$. The union of the finite partial elementary maps is an elementary embedding $M\to N$. Hence $M$ is prime.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
