<h1 id="d7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\xi_j$ be the displacement in step $j$, so the [random walk](../../../../../random-walk-split.md) position is $x(n)=\sum_{j=1}^n\xi_j$. The single-step [expected value](../../../../../expected-value-split.md) and second [moment](../../../../../moment.md) are

$$
\mathbb E[\xi_j]=\tfrac13\delta-\tfrac13\delta+\tfrac13(0)=0,\qquad
\mathbb E[\xi_j^2]=\tfrac13\delta^2+\tfrac13\delta^2=\tfrac23\delta^2.
$$

By linearity of [expected value](../../../../../expected-value-split.md), **$\boxed{\langle x(n)\rangle=0}$.** The steps are [independent random variables](../../../../../independent-random-variables.md), so for $i\ne j$, $\mathbb E[\xi_i\xi_j]=\mathbb E[\xi_i]\mathbb E[\xi_j]=0$. Expanding the square gives the [mean squared displacement](../../../../../mean-squared-displacement.md)

$$
\boxed{\langle x^2(n)\rangle=\sum_{j=1}^n\mathbb E[\xi_j^2]
+2\sum_{i<j}\mathbb E[\xi_i\xi_j]=\frac23n\delta^2}.
$$

These are ensemble [expected values](../../../../../expected-value-split.md); the empirical average over a finite number $N$ of independent cells fluctuates about them. The expected [mean squared displacement](../../../../../mean-squared-displacement.md) itself does not depend on $N$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [D7](../../d7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
