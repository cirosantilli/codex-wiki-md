<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each $X_i$ has the same [probability distribution](../../../../../../../probability-distribution-split.md) as $-X_i$, and [independence](../../../../../../../independent-random-variables.md) makes $S_m$ and $-S_m$ identically distributed. Thus their two strict tail [probabilities](../../../../../../../probability.md) are equal:

$$
\mathbb P(S_m>m/2)=\mathbb P(S_m<-m/2)=\frac12\mathbb P(|S_m|>m/2).
$$

Apply [Chebyshev's inequality](../../../../../../../chebyshev-s-inequality.md) using the [mean](../../../../../../../expected-value-split.md) and [variance](../../../../../../../variance-split.md) from part (i):

$$
\boxed{\mathbb P(S_m>m/2)\leq\frac12\frac{2m/3}{(m/2)^2}=\frac4{3m}.}
$$

The equal-tail argument is essential: applying [Chebyshev's inequality](../../../../../../../chebyshev-s-inequality.md) directly to the absolute tail alone gives the weaker bound $8/(3m)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
