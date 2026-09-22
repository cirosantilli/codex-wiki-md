<h1 id="m/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $n=0$, the identity [matrix](../../../../../matrix.md) gives the assertion. Suppose it holds at $n$. Conditioning on the state at time $n$ and using the [Markov property](../../../../../markov-property.md) gives

$$
\mathbb P(X_{n+1}=j\mid X_0=i)
=\sum_k\mathbb P(X_n=k\mid X_0=i)P_{kj}
=\sum_k(P^n)_{ik}P_{kj}=(P^{n+1})_{ij}.
$$

The nonnegative countable sum is justified by the law of total probability. Induction proves **the $n$-step [transition matrix](../../../../../stochastic-matrix.md) is $P^n$**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [M](../../../m.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
