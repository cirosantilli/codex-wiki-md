<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [coalition](../../../../../../coalition-game-theory.md) $S$, its [coalition excess](../../../../../../excess-of-a-coalition.md) at an allocation is $e(S,x)=v(S)-x(S)$, measuring its complaint. Sort all these [excesses of a coalition](../../../../../../excess-of-a-coalition.md) in decreasing order. The [nucleolus](../../../../../../nucleolus.md) is the [imputation](../../../../../../imputation-in-a-coalitional-game.md) whose sorted [vector](../../../../../../vector.md) is smallest in [lexicographic order](../../../../../../lexicographic-order.md): minimize the greatest complaint first, then the next among ties, and continue. Including the empty and grand [coalitions](../../../../../../coalition-game-theory.md) merely inserts two fixed zero entries and does not change the minimizing allocation.

For every efficient allocation, the [excesses of a coalition](../../../../../../excess-of-a-coalition.md) of $\{2\}$ and $\{1,3\}$ sum to zero:

$$
e(\{2\},x)+e(\{1,3\},x)
=2-x_2+10-(12-x_2)=0.
$$

The largest proper-coalition [coalition excess](../../../../../../excess-of-a-coalition.md) is therefore at least zero. Since the [core of a cooperative game](../../../../../../core-game-theory.md) from part (b) is nonempty, this first-stage minimum is exactly zero and its minimizers are precisely that [core of a cooperative game](../../../../../../core-game-theory.md). Restrict to $x=(t,2,10-t)$, $1\le t\le6$. The six proper-coalition [excesses of a coalition](../../../../../../excess-of-a-coalition.md) are

$$
\begin{array}{c|rrrrrr}
S&1&2&3&12&13&23\\ \hline
e(S,x)&1-t&0&t-7&1-t&0&t-6
\end{array}
$$

The two zero [excesses of a coalition](../../../../../../excess-of-a-coalition.md) are fixed. Among the remaining [excesses of a coalition](../../../../../../excess-of-a-coalition.md), $t-7<t-6$, so the next largest complaint is $\max\{1-t,t-6\}$. It is minimized by equalizing those two affine expressions:

$$
1-t=t-6,\qquad t=\frac72,\qquad
\max\{1-t,t-6\}=-\frac52.
$$

This minimizer is unique, so later lexicographic stages cannot change it. Thus

$$
\boxed{\nu(v)=\left(\frac72,2,\frac{13}{2}\right).}
$$

Its sorted proper-coalition [coalition excess](../../../../../../excess-of-a-coalition.md) [vector](../../../../../../vector.md) is $(0,0,-5/2,-5/2,-5/2,-7/2)$. The calculation both identifies the [nucleolus](../../../../../../nucleolus.md) and proves uniqueness for this game without replacing the requested computation by the general uniqueness theorem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
