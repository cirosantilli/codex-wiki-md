<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The initial values of the two [sequences](../../../../../sequence.md) agree: $c_0=d_0=1$ and $c_1=-1+c_0=0=d_1$. For $n\geq2$, use the first-order [recurrence relation](../../../../../recurrence-relation.md) at $n$ and $n-1$:

$$
\begin{aligned}
c_n-(n-1)(c_{n-1}+c_{n-2})
&=(-1)^n+c_{n-1}-(n-1)c_{n-2}\\
&=(-1)^n+(-1)^{n-1}=0.
\end{aligned}
$$

Therefore $c_n$ satisfies exactly the same [derangement recurrence](../../../../../derangement-recurrence.md) as $d_n$. By [strong induction](../../../../../strong-induction.md), equality of the preceding two terms implies equality of the next term. Consequently

$$
\boxed{c_n=d_n\quad\text{for every }n\geq0.}
$$

The first-order [recurrence relation](../../../../../recurrence-relation.md) therefore also counts [derangements](../../../../../derangement-of-a-permutation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
