<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $d=-c>0$. Suppose, for a contradiction, that only finitely many sign changes occur. Since every $a_n\ne0$, the sign is then constant for $n\geq N$. Set $b_n=|a_n|>0$ on that tail. Multiplying the [recurrence relation](../../../../../../../recurrence-relation.md) by this constant sign gives

$$
b_{n+1}=\frac12\left(b_n-\frac d{b_n}\right)>0,
\qquad 0<b_{n+1}<\frac12b_n.
$$

Consequently $b_{N+j}<2^{-j}b_N$ for $j\geq1$, and $b_n\to0$ by comparison with a [geometric sequence](../../../../../../../geometric-progression.md). But positivity of $b_{n+1}$ requires $b_n^2>d$ at every step, which is incompatible with $b_n\to0$. Thus the [negative-parameter square-root iteration changes sign infinitely often](../../../../../../../negative-parameter-square-root-iteration-changes-sign-infinitely-often.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
