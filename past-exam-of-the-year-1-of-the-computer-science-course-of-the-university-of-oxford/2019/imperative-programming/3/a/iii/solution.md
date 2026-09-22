<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Regardless of which branch is taken, $r(n)\leq r(n-1)+n$. Starting from zero and applying [induction](../../../../../../mathematical-induction.md) gives

$$
\boxed{0\leq r(n)\leq\sum_{i=1}^{n}i=\frac{n(n+1)}2.}
$$

For the inductive step, add $n$ to the bound $(n-1)n/2$ for the previous value. The subtraction branch gives an even smaller result, and positivity is checked there. This bound need not describe the actual growth sharply; it is sufficient to size a finite membership representation for a requested prefix.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
