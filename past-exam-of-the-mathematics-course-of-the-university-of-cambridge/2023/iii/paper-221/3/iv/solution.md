<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $M$ be a Markov blanket of the treatment $A$ inside $(A,X)$, and write the remaining adjustment variables as $N=X\setminus M$. By definition,

$$
A\perp N\mid M.
$$

The sufficiency of $X=(M,N)$ gives

$$
A\perp Y(a)\mid(M,N).
$$

Apply the [contraction axiom for conditional independence](../../../../../../contraction-axiom-for-conditional-independence.md) with first variable $A$, second variable $N$, third variable $Y(a)$, and conditioning variable $M$. It gives

$$
A\perp(N,Y(a))\mid M.
$$

The [decomposition axiom for conditional independence](../../../../../../decomposition-axiom-for-conditional-independence.md) then yields $A\perp Y(a)\mid M$. Hence every Markov blanket of $A$ in $(A,X)$ is itself a [sufficient adjustment set](../../../../../../sufficient-adjustment-set.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
