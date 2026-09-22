<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Enumerate the countable atomic model as $M=\{a_0,a_1,\ldots\}$ and fix any $N\models T$. We recursively construct finite partial elementary maps $f_n$ from the first $n$ elements of $M$ into $N$.

Suppose $f_n(\bar a)=\bar b$. Since $M$ is atomic, choose a formula $\theta(\bar x,y)$ isolating $\operatorname{tp}(\bar a,a_n)$. Its existential consequence $\exists y\,\theta(\bar x,y)$ belongs to $\operatorname{tp}(\bar a)$, so partial elementarity gives

$$
N\models\exists y\,\theta(\bar b,y).
$$

Choose a witness $b_n$. Because $\theta$ isolates the complete joint type, extending $f_n$ by $a_n\mapsto b_n$ remains partial elementary. The union of the recursive maps is an elementary embedding $M\to N$. Thus every countable atomic model is a [prime model](../../../../../../prime-model.md), proving the [countable atomic model is prime](../../../../../../countable-atomic-model-is-prime.md) result.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 144](../../../paper-144-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
