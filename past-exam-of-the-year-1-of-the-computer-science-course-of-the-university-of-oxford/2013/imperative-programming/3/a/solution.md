<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $a_0$ be a saved mathematical copy of the original [array](../../../../../array-data-structure.md). A precise [postcondition](../../../../../postcondition.md) for [sorting](../../../../../sorting.md) is

$$
\boxed{\begin{aligned}
&\forall i,j\in[0,N):\ i<j\Longrightarrow a(i)\leq a(j),\\
&\forall v\in\mathbb Z:\ \#\{i:a(i)=v\}=\#\{i:a_0(i)=v\}.
\end{aligned}}
$$

The [precondition](../../../../../precondition.md) is that `a` is a non-null [array](../../../../../array-data-structure.md) of length $N\geq0$. Its length and every unrelated object remain unchanged. The second clause preserves the [array multiset](../../../../../array-multiset.md), including all multiplicities; ordering alone would also permit overwriting the entire [array](../../../../../array-data-structure.md) with zeros. The saved $a_0$ is a specification device and need not be allocated by the implementation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
