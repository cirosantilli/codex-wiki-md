<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write the input [word over an alphabet](../../../../../../string.md) as $w=a_1\cdots a_n$. Starting with $z_0=\gamma$, obtain $z_i$ from $z_{i-1}$ by [linear-time multiplication in an automatic structure](../../../../../../linear-time-multiplication-in-an-automatic-structure.md) with $a_i$. [Mathematical induction](../../../../../../mathematical-induction.md) gives

$$
z_i\in L,\qquad \overline{z_i}=a_1\cdots a_i,
\qquad |z_i|\leq|\gamma|+iN.
$$

The [time complexity](../../../../../../time-complexity.md) of step $i$ is at most a constant times $|\gamma|+(i-1)N+1$. Summing the costs gives

$$
T(w)\leq C\sum_{i=1}^n\bigl(|\gamma|+(i-1)N+1\bigr)
=C\left(n(|\gamma|+1)+\frac{Nn(n-1)}2\right).
$$

The [automatic structure for a group](../../../../../../automatic-structure-for-a-group.md), $N$ and $\gamma$ are fixed, so **the required representative is**

$$
\boxed{z=z_n,\qquad \overline z=\overline w,\qquad
|z|\leq |\gamma|+nN,\qquad T(w)=O(n^2)\ (n\geq1).}
$$

For the [empty word](../../../../../../empty-word.md), return $\gamma$ in constant time.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
