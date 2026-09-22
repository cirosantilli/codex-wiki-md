<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $N$ beyond every [peak of a sequence](../../../../../../../peak-of-a-sequence.md) of both $(a_n)$ and $(-a_n)$. Every term with index at least $N$ has a strictly larger later term and a strictly smaller later term.

Suppose for a contradiction that $a_n\to L$. Starting at $a_N$, recursively select a strictly increasing [subsequence](../../../../../../../subsequence.md) and a strictly decreasing [subsequence](../../../../../../../subsequence.md). Both must have [limit of a sequence](../../../../../../../limit-of-a-sequence.md) $L$. If their second terms are $u>a_N$ and $v<a_N$, respectively, passage to their [limits of sequences](../../../../../../../limit-of-a-sequence.md) gives

$$
L\geq u>a_N,\qquad L\leq v<a_N,
$$

a contradiction. Hence **$(a_n)$ does not converge.** This argument includes the possibility that either [set](../../../../../../../set-split.md) of [peaks of a sequence](../../../../../../../peak-of-a-sequence.md) is empty.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
