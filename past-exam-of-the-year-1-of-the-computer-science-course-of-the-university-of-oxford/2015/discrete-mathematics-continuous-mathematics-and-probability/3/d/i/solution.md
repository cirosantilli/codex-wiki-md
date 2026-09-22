<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider one iteration with $a_i>b_i>0$ and $r_i=a_i\bmod b_i$. If $b_i\le a_i/2$, then $r_i<b_i\le a_i/2$. If $b_i>a_i/2$, the [quotient](../../../../../../quotient.md) is $1$, so $r_i=a_i-b_i<a_i/2$. In either case $r_i<a_i/2$, whence

$$
a_{i+1}b_{i+1}=b_ir_i<\frac{a_ib_i}{2}.
$$

Repeated application, or [mathematical induction](../../../../../../mathematical-induction.md), proves

$$
\boxed{a_nb_n<\frac{ab}{2^n}\qquad(n\ge1\text{ performed iterations}).}
$$

This also holds for the final iteration, whose left side is zero. For zero iterations the correct relation is equality $a_0b_0=ab$, rather than a strict [inequality](../../../../../../inequality-mathematics.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
