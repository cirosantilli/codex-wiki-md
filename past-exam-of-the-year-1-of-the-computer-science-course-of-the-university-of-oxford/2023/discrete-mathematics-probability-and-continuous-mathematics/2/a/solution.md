<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [strong induction](../../../../../strong-induction.md) with three consecutive base cases:

$$
8=3+5,\qquad9=3\cdot3,\qquad10=5\cdot2.
$$

For $n\ge11$, assume all values from $8$ through $n-1$ have the required representation. Since $8\le n-3<n$, write $n-3=3k+5m$ with $k,m$ [nonnegative integers](../../../../../natural-number.md). Then $n=3(k+1)+5m$ is another such representation. [Strong induction](../../../../../strong-induction.md) proves the claim for every $n\ge8$. This is a [consecutive-base induction for additive semigroups](../../../../../consecutive-base-induction-for-additive-semigroups.md): the three base cases handle all residues before repeated addition of $3$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
