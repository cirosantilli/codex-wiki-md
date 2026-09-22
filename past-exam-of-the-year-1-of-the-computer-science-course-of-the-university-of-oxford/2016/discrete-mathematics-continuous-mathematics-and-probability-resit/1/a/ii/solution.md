<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Using [set difference](../../../../../../set-difference.md) as intersection with a [complement of a set](../../../../../../complement-of-a-set.md), then [De Morgan's laws](../../../../../../de-morgan-s-laws.md) and distribution, gives

$$
\begin{aligned}
(A\cup B)\setminus(C\setminus A)
&=(A\cup B)\cap(C\cap A^c)^c\\
&=(A\cup B)\cap(C^c\cup A)\\
&=A\cup(B\cap C^c)\\
&=\boxed{A\cup(B\setminus C)}.
\end{aligned}
$$

For the third equality, expand the two [set unions](../../../../../../set-union.md): the terms $A\cap C^c$ and $A\cap B$ are absorbed by $A$, and $A\cap A=A$. This proves the required identity entirely by [set](../../../../../../set-split.md) algebra.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
