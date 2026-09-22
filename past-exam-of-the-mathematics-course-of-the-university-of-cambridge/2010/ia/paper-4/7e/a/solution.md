<h1 id="7e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Enumerate $A$ as $a_1,\ldots,a_a$. A [function](../../../../../../function-split.md) is specified by choosing the image of each of these elements independently, with $b$ possibilities each. The [multiplication principle](../../../../../../rule-of-product.md) gives $\boxed{b^a\text{ functions}}$.

For an [injective function](../../../../../../injective-function.md), successive images must be distinct. If $a\le b$, there are $b$ choices for the first, $b-1$ for the second, and so on. If $a>b$, the [pigeonhole principle](../../../../../../pigeonhole-principle.md) makes injectivity impossible. Thus the number of [injective functions](../../../../../../injective-function.md) is

$$
\boxed{\begin{cases}
\displaystyle b(b-1)\cdots(b-a+1)=\frac{b!}{(b-a)!},&a\le b,\\
0,&a>b.
\end{cases}}
$$

The product in the first case is a [falling factorial](../../../../../../falling-factorial.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
