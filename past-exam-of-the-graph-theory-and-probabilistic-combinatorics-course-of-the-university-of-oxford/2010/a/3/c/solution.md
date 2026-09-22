<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Verify [Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md). Let $S\subseteq X$; the empty case is immediate. If $0<|S|\leq\epsilon n$, any $x\in S$ has at least $\epsilon n$ neighbors in $Y$, so $|N(S)|\geq|S|$.

Next suppose $\epsilon n<|S|\leq(1-\epsilon)n$. If $|N(S)|<|S|$, then $T=Y\setminus N(S)$ has $|T|>n-|S|\geq\epsilon n$. There are no edges between $S$ and $T$, so $d(S,T)=0$. But the [regularity](../../../../../regular-pair-of-vertex-sets.md) assumption implies

$$
d(S,T)\geq d(X,Y)-\epsilon>0,
$$

a contradiction.

Finally, if $|S|>(1-\epsilon)n$, then $|X\setminus S|<\epsilon n$. Every $y\in Y$ has at least $\epsilon n$ neighbors in $X$, so at least one of them lies in $S$. Thus $N(S)=Y$ and $|N(S)|=n\geq|S|$.

All possible sizes of $S$ are covered, even if the middle range is empty. Hall's condition holds, so **there is a [perfect matching](../../../../../perfect-matching.md) between $X$ and $Y$**. This is the [perfect matching criterion for a regular pair with minimum degree](../../../../../perfect-matching-criterion-for-a-regular-pair-with-minimum-degree.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
