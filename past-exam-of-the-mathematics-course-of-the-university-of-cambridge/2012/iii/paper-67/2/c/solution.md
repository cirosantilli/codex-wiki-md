<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First use the allowed one-query algorithm to learn $p=x_1\mathbin\oplus x_2$ exactly. This restricted two-index [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) is realized by relabelling indices $1,2$ in a single query to the original input. Measure its output and choose the second query classically.

If $p=0$, the first two bits agree and their common value is the majority, irrespective of $x_3$. Query $x_1$ and output it. If $p=1$, the first two bits cancel in the vote, so query $x_3$ and output it. Thus

$$
\boxed{\operatorname{MAJ}(x)=\begin{cases}x_1,&x_1\oplus x_2=0,\\x_3,&x_1\oplus x_2=1.\end{cases}}
$$

The [exact two-query majority algorithm](../../../../../../exact-two-query-majority-algorithm.md) uses one parity query and one ordinary bit query on every branch, and is correct on all eight inputs. Together with the lower bound this proves **$Q_E(\operatorname{MAJ})=2$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
