<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $C^c=\mathcal U\setminus C$. The rules for [set difference](../../../../../../set-difference.md), [set intersection](../../../../../../set-intersection.md), and [complement of a set](../../../../../../complement-of-a-set.md) give

$$
\begin{aligned}
(A\cap B)\setminus(A\cap C)
&=(A\cap B)\cap(A\cap C)^c\\
&=(A\cap B)\cap(A^c\cup C^c)\\
&=(A\cap B\cap A^c)\cup(A\cap B\cap C^c)\\
&=\varnothing\cup\bigl(A\cap(B\cap C^c)\bigr)\\
&=\boxed{A\cap(B\setminus C)}.
\end{aligned}
$$

The second step is [De Morgan's laws](../../../../../../de-morgan-s-laws.md); the third distributes [set intersection](../../../../../../set-intersection.md) over [set union](../../../../../../set-union.md). The fourth uses $A\cap A^c=\varnothing$.

## ↑ Ancestors (13)

1. [I](../i.md)
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
