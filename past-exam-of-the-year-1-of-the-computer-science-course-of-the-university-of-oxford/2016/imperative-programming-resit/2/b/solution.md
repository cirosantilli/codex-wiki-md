<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [partitions into distinct parts](../../../../../partition-into-distinct-parts.md), using a part $i$ prevents using it again. Hence

$$
\boxed{d(i,n)=d(i-1,n)+d(i-1,n-i)}
$$

when $1\leq i\leq n$, with $d(i,0)=1$, $d(0,n)=0$ for $n>0$, and $d(i,n)=0$ for $n<0$. When $i>n$, use $d(i,n)=d(i-1,n)$. Thus change the second call in the final branch of `P` to `D(i-1, n-i)` and rename all calls to `D`. The same split into two disjoint classes proves correctness; its second class removes its unique largest allowed part. **The answer is $D(n,n)$**, giving $D(4,4)=2$, from $4$ and $3+1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
