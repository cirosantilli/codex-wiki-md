<h1 id="b/6/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The full-cycle formula says that precisely the nonhook shapes have zero value on a 6-cycle. These are $(4,2),(3,3),(3,2,1),(2,2,1,1),(2,2,2)$.

Use the standard two-row permutation-[character](../../../../../character-of-a-representation.md) rule $\pi^{(6-r,r)}=\chi^{(6)}+\chi^{(5,1)}+\cdots+\chi^{(6-r,r)}$. A transposition has four fixed points, so $\chi^{(5,1)}=3$. It fixes $\binom42+1=7$ two-subsets, giving $\chi^{(4,2)}=7-1-3=3$. It fixes $\binom43+\binom41=8$ three-subsets, giving $\chi^{(3,3)}=8-1-3-3=1$.

Conjugating a partition tensors its [character](../../../../../character-of-a-representation.md) with the sign [character](../../../../../character-of-a-representation.md). Hence the values on a transposition for the conjugate shapes are $-3$ and $-1$. The shape $(3,2,1)$ is self-conjugate, so its [character](../../../../../character-of-a-representation.md) equals its own sign twist and is zero on every odd permutation. The complete candidate table is therefore:

| Shape | Value on a transposition |
| --- | --- |
| $(4,2)$ | $3$ |
| $(3,3)$ | $1$ |
| $(3,2,1)$ | $0$ |
| $(2,2,1,1)$ | $-3$ |
| $(2,2,2)$ | $-1$ |

Thus the unique answer is

$$
\boxed{\lambda=(3,2,1).}
$$

## ↑ Ancestors (13)

1. [3](../3.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
