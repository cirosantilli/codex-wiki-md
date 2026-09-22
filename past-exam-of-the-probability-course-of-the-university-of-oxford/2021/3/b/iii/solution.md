<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose a [stationary distribution](../../../../../stationary-distribution.md) $\pi$ exists. Its [stationarity equations](../../../../../stationarity-equations.md) are

$$
\pi_j=p\pi_{j-a}+q\pi_{j+b}\qquad(j\in\mathbb Z).
$$

Since $\sum_j\pi_j=1$, its masses tend to zero as $|j|\to\infty$, and a positive maximum $M=\pi_{j_0}$ is attained. Both terms on the right are at most $M$. Since $p,q>0$ and $p+q=1$, equality forces $\pi_{j_0-a}=\pi_{j_0+b}=M$. Applying the same argument repeatedly at $j_0-a,j_0-2a,\ldots$ gives

$$
\pi_{j_0-ka}=M>0\qquad(k\geq0).
$$

These are infinitely many distinct states, contradicting $\sum_j\pi_j=1$. Thus

$$
\boxed{\text{There is no stationary distribution.}}
$$

This [maximum principle](../../../../../maximum-principle.md) proof uses neither a finite [expected value](../../../../../expected-value-split.md) of the state nor the [coprimality](../../../../../coprime-integers.md) assumption.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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
