<h1 id="3f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every allocation is determined by the set of $n$ children on the red bus, so there are $\binom{2n}{n}$ equally likely allocations. Exactly one places every boy on red and every girl on green. Hence

$$
\mathbb P(A_n)=\binom{2n}{n}^{-1}=\frac{(n!)^2}{(2n)!}.
$$

Applying [Stirling formula](../../../../../../stirling-formula.md) to the numerator and denominator gives the [central binomial coefficient](../../../../../../central-binomial-coefficient.md) asymptotic

$$
\binom{2n}{n}\sim\frac{4^n}{\sqrt{\pi n}},
$$

and therefore

$$
\boxed{\mathbb P(A_n)\sim\frac{\sqrt{\pi n}}{4^n}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3F](../../3f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
