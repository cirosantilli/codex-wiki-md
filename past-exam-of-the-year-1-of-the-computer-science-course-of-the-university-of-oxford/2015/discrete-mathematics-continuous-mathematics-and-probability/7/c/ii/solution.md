<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each $X_i$ has the same [probability distribution](../../../../../../probability-distribution-split.md) as $-X_i$. By [independence](../../../../../../independent-random-variables.md), the entire vector and its negative have the same joint law, so $S_m$ has a [symmetric distribution](../../../../../../symmetric-distribution.md) about zero. The two disjoint tail [events](../../../../../../event.md) consequently have equal [probabilities](../../../../../../probability.md):

$$
\mathbb P(S_m>m/2)=\mathbb P(S_m<-m/2)
=\frac12\mathbb P(|S_m|>m/2).
$$

Apply [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) with the [mean](../../../../../../expected-value-split.md) and [variance](../../../../../../variance-split.md) from (i):

$$
\mathbb P(S_m>m/2)
\le\frac12\frac{2m/3}{(m/2)^2}
=\boxed{\frac4{3m}}.
$$

Using only containment in the two-sided event would give $8/(3m)$; the [symmetry](../../../../../../symmetry-physics.md) supplies the necessary extra factor $1/2$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
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
