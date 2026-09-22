<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Enumerate both [sets](../../../../../../../set-split.md) of [peaks of a sequence](../../../../../../../peak-of-a-sequence.md) in increasing order of index. If $a_n\to L$, the two selected [subsequences](../../../../../../../subsequence.md) both tend to $L$.

For the converse, suppose $a_{k_r}\to L$ and $a_{m_r}\to L$. Given $\varepsilon>0$, choose $r$ large enough that both selected terms differ from $L$ by less than $\varepsilon$. For every $n>\max\{k_r,m_r\}$, the two [peak of a sequence](../../../../../../../peak-of-a-sequence.md) conditions imply

$$
\boxed{L-\varepsilon<a_{m_r}\leq a_n\leq a_{k_r}<L+\varepsilon.}
$$

The lower bound comes from the [peak of a sequence](../../../../../../../peak-of-a-sequence.md) of $(-a_n)$ at $m_r$. This is precisely the definition of $a_n\to L$. Thus **convergence is equivalent to a common finite [limit of a sequence](../../../../../../../limit-of-a-sequence.md) for the upper and lower peak [subsequences](../../../../../../../subsequence.md).**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
