<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $T_0=0$ and $E_j=T_j-T_{j-1}$. The [Poisson interarrival times](../../../../../poisson-interarrival-times.md) $E_j$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with the rate-one [exponential distribution](../../../../../exponential-distribution.md). In particular, $\mathbb EE_j=1$ and $\operatorname{Var}(E_j)=1$, so the finite, positive [variance](../../../../../variance-split.md) hypothesis of the [central limit theorem](../../../../../central-limit-theorem.md) holds. Since $T_n=\sum_{j=1}^nE_j$,

$$
\boxed{\frac{T_n-n}{\sqrt n}=\frac1{\sqrt n}\sum_{j=1}^n(E_j-1)\ \xrightarrow{\mathrm d}\ N(0,1).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
