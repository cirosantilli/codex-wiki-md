<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [De Morgan's laws](../../../../../de-morgan-s-laws.md) to remove the [complement of a set](../../../../../complement-of-a-set.md), then distribute the two [unions](../../../../../set-union.md):

$$
\begin{aligned}
(A\cup B)\setminus(A\cap B)
&=(A\cup B)\cap(\overline A\cup\overline B)\\
&=(A\cap\overline A)\cup(A\cap\overline B)\cup(B\cap\overline A)\cup(B\cap\overline B)\\
&=(A\cap\overline B)\cup(B\cap\overline A).
\end{aligned}
$$

The first and last [intersections](../../../../../set-intersection.md) in the middle line are the [empty set](../../../../../empty-set.md). The remaining [union](../../../../../set-union.md) is precisely the collection of elements belonging to exactly one of the original [sets](../../../../../set-split.md). Therefore both expressions define the same [symmetric difference](../../../../../symmetric-difference.md):

$$
\boxed{(A\cup B)\setminus(A\cap B)=(A\setminus B)\cup(B\setminus A)=A\oplus B.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
