<h1 id="d/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Lebesgue outer measure](../../../../lebesgue-outer-measure.md) of $E$ is the infimum of $\sum_j|I_j|$ over countable coverings by open intervals. A set is a [null set](../../../../null-set.md) when this infimum is zero, equivalently when it has such a cover of total length less than every prescribed positive number.

The [Cantor set](../../../../cantor-set.md) is obtained from $[0,1]$ by deleting the open middle third of every remaining interval at each stage. After $n$ stages it lies inside $2^n$ closed intervals of length $3^{-n}$. Slightly enlarging these finitely many intervals to open intervals shows its [outer measure](../../../../outer-measure.md) is at most $(2/3)^n$ for every $n$, hence zero.

For the modified construction, let $L_n$ be the total length of the $2^n$ intervals in $K_n$. The removed fraction at stage $n$ is exactly $1/(2^n+2)$, so

$$
L_{n+1}=L_n\frac{2^n+1}{2^n+2},\qquad L_0=1.
$$

The product telescopes because $2^n+2=2(2^{n-1}+1)$, giving

$$
L_n=\frac13+\frac{2}{3\cdot2^n}.
$$

Since $K\subseteq K_n$, the same finite interval-cover argument gives $m^*(K)\leq L_n$ for every $n$. Taking the infimum proves

$$
\boxed{m^*(K)\leq1/3.}
$$

Only interval lengths and the definition of [outer measure](../../../../outer-measure.md) were used; the three numbered clauses in the source describe the construction rather than separate requests to prove additional statements.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [D](../../d.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
