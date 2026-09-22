<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) handles small base cases directly, divides a larger instance into smaller instances of the same problem, solves them recursively, and combines their answers. The savings come from the number and sizes of recursive calls and the combination cost.

For [Karatsuba multiplication](../../../../../karatsuba-multiplication.md), split the $n$-bit inputs as $x=aB+b$, $y=cB+d$, where $B=2^k$ and $k=\lceil n/2\rceil$. Compute only three recursive products:

$$
p=ac,\qquad q=bd,\qquad r=(a-b)(c-d).
$$

Then the [Karatsuba three-product identity](../../../../../karatsuba-three-product-identity.md) gives

$$
\boxed{xy=pB^2+(p+q-r)B+q.}
$$

The absolute differences have at most $k$ bits; multiply their magnitudes and restore the sign of $r$. Additions, subtractions and shifts cost $O(n)$ bit operations. With constant-size base cases, the [recurrence relation](../../../../../recurrence-relation.md) is $T(n)=3T(\lceil n/2\rceil)+O(n)$, giving **$O(n^{\log_2 3})$** by the [Master theorem](../../../../../master-theorem.md). The difference-product version avoids an extra carry bit in the recursive operands.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
