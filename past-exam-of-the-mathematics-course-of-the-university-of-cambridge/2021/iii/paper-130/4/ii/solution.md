<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume condition i and call a set $B\subseteq\mathbb N$ bad when it contains no member of $\mathcal S$. No finite collection of bad sets covers $\mathbb N$: if it did, assigning each integer to the first bad set containing it would give a finite coloring whose color classes are bad, contrary to condition i. Consequently

$$
\{\mathbb N\setminus B:B\text{ is bad}\}
$$

has the finite-intersection property. It generates a proper [filter on a set](../../../../../../filter-set-theory.md), which the [ultrafilter lemma](../../../../../../ultrafilter-lemma.md) extends to an ultrafilter $\mathcal U$. If some $A\in\mathcal U$ were bad, then $\mathbb N\setminus A$ would also belong to $\mathcal U$ by construction, contradicting propriety. Hence every $A\in\mathcal U$ contains a member of $\mathcal S$, proving condition ii.

For the final question, let $\mathcal S$ consist of the pairs $\{x,2x\}$ and $\{x,3x\}$. Color $n$ by

$$
v_2(n)+v_3(n)\pmod2.
$$

Multiplication by either two or three reverses this parity, so this two-coloring has no monochromatic member of $\mathcal S$. Condition i fails, and the equivalence just proved shows that no ultrafilter with the stated property exists.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
