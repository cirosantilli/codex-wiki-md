<h1 id="m/m5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $n=0$, the transition probabilities are the entries of the identity $P^0$. Suppose the formula holds for $n$. Conditioning on $X_n=k$ and using the [Markov property](../../../../../markov-property.md) gives

$$
P(X_{n+1}=j\mid X_0=i)
=\sum_{k\in S}P(X_n=k\mid X_0=i)P_{kj}
=\sum_k(P^n)_{ik}P_{kj}=(P^{n+1})_{ij}.
$$

The countable sums have nonnegative terms, so they are justified by the [law of total probability](../../../../../law-of-total-probability.md). Induction proves

$$
\boxed{P(X_n=j\mid X_0=i)=(P^n)_{ij}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
