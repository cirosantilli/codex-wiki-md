<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $U'=U\setminus\{y\}$ and $\mathcal F'=\{B\setminus\{y\}:B\in\mathcal F\}$. If $\mathcal A$ is a basis for the original instance, replace each member $A$ by $A\setminus\{y\}$. Deletion commutes with [unions](../../../../../../set-union.md), so the resulting family generates every member of $\mathcal F'$ and has at most $|\mathcal A|$ members.

Conversely, take a basis $\mathcal A'$ for the reduced instance. Lift each of its members by

$$
L(A')=\begin{cases}A'\cup\{y\},&x\in A',\\A',&x\notin A'.\end{cases}
$$

If $B\setminus\{y\}$ is represented as a [union](../../../../../../set-union.md) of reduced basis [sets](../../../../../../set-split.md), the same [union](../../../../../../set-union.md) of their lifts agrees with $B$ on $U'$. It contains $y$ exactly when one of the selected reduced basis [sets](../../../../../../set-split.md) contains $x$, namely exactly when $x\in B$. By the assumed [incidence equivalence in a set family](../../../../../../incidence-equivalence-in-a-set-family.md), this occurs exactly when $y\in B$. Thus the lifted [union](../../../../../../set-union.md) is precisely $B$, and the lifted basis has no more members.

Therefore **deleting $y$ preserves the yes/no answer with the same parameter $k$**. The reverse construction does not require a reduced basis [set](../../../../../../set-split.md) to be an input [set](../../../../../../set-split.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Algorithms](../../../../algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
